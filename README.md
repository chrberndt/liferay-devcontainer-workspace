# liferay-devcontainer-workspace

A Liferay DXP workspace meant to explore and demonstrate how to use devcontainers as unified development environment.

# Prerequisites

A valid GitHub account. GitHub currently (September 2026) offers access to codespaces within the free tier, see: https://github.com/pricing.

# Usage

## Setup 

1. Fork the repo to your account.
1. Click the green "Code" button and switch to the "Codespaces" tab.
1. Click the green "Create codespace on main" button
1. When prompted, hit "Trust Folder & Continue"

## Run Liferay

1. Copy your developer license to `config/common/osgi/modules` (Please note: the license key should reside only in your codespace or a private repo but not in a publicly accessible repository.)
1. From the Gradle view, choose Tasks → bundle → initBundle or run `./gradlew initBundle` from the terminal to setup your development server.
1. Subsequently you can run Liferay by issuing `./bundles/tomcat/bin/catalina.sh jpda run` like you would do in a local environment.
1. Switch to the "Ports" tab and use the "Open in Browser" globe icon to access your Liferay development server.

## Scaffold and deploy "traditional" OSGi modules with blade

TODO

## Create and deploy client extensions

TODO

# Feedback, Questions, and Suggestions

christian.berndt@liferay.com
