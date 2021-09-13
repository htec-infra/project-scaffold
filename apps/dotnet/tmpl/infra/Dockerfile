ARG DOTNET_VERSION=3.1

#====================================================================
#               Buildtime Image
#====================================================================
FROM mcr.microsoft.com/dotnet/core/sdk:${DOTNET_VERSION}-buster AS build-env
WORKDIR /app

# Copy csproj and restore as distinct layers
COPY ./src ./

# Run Unit Tests
# RUN dotnet test App.sln -c Release --logger:console\;verbosity=normal

# Restore / Build and publish Reporter API including all dependencies
# RUN dotnet publish App/App.csproj -c Release -o dist

#====================================================================
#               Runtime Image
#====================================================================
FROM mcr.microsoft.com/dotnet/core/aspnet:${DOTNET_VERSION}-buster-slim
ARG VERSION=alpha
ARG REVISION=abcdefg

WORKDIR /app

#LABEL vendor="HTEC Group Inc."
#LABEL maintainer="HTEC Group Inc."
#LABEL com.htecgroup.app_category="API"
#LABEL com.htecgroup.app_repository="<org>/<app-repo>"

ENV APP_NAME="Full Application Name"
ENV APP_VERSION=${VERSION}
ENV APP_REVISION=${REVISION}

# Copy application runtime DLLs
COPY --from=build-env /app/dist .
#
# ENTRYPOINT ["dotnet", "App.dll"]
