# Azure 3-Tier Architecture

## Project Overview
A full 3-tier cloud architecture deployed on Microsoft Azure.

## Architecture
- **Tier 1 - Presentation:** Azure App Service (frontend)
- **Tier 2 - Application:** Azure App Service with VNet Integration
- **Tier 3 - Data:** Azure SQL Database

## Services Used
- Azure App Service
- Azure SQL Database
- Azure Virtual Network (VNet)
- Network Security Groups (NSGs)
- Azure App Service Plan

## Network Design
- VNet: 10.0.0.0/16
- subnet-frontend: 10.0.1.0/24
- subnet-backend: 10.0.2.0/24
- subnet-database: 10.0.3.0/24

## Security
- nsg-frontend: Allows HTTP (80) and HTTPS (443) from internet
- nsg-backend: Allows traffic from frontend subnet only (port 8080)
- nsg-database: Allows traffic from backend subnet only (port 1433)

## Live URL
https://app-3tier-kinjal-dwcaeeh8enetggha.italynorth-01.azurewebsites.net

## What I Learned
- How to design and deploy a 3-tier architecture on Azure
- How to secure traffic between tiers using NSGs
- How to configure VNet subnets for network isolation
- How Azure App Service connects to backend databases securely

## Region
North Italy (Azure for Students subscription)
