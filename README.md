# YARP Reverse Proxy  

This repository contains a .NET project for a reverse proxy built using [YARP (Yet Another Reverse Proxy)](https://microsoft.github.io/reverse-proxy/).  
See this on [Microsoft](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/servers/yarp/yarp-overview?view=aspnetcore-9.0).

## Project Structure  

- **`Yarp.ReverseProxy`**:  
    The main project implementing the reverse proxy. It is configured to use .NET 9.0 and includes the following key components:  
    - `Program.cs`: Sets up the reverse proxy using configuration from `appsettings.json`.  
    - `appsettings.json`: Contains the configuration for routes and clusters used by the reverse proxy.  


## Key Features  

- **Reverse Proxy Configuration**:  
    - Routes and clusters are defined in `appsettings.json`.  
    - Routes include options for authorization policies, rate-limiting, and path transformations.  
    - Clusters define destinations and load-balancing policies.  

## Dependencies  

- **NuGet Packages**:  
    - `Yarp.ReverseProxy` (v2.3.0): Provides reverse proxy functionality.  

## Configuration  

- **Routes**: Define how incoming requests are matched and routed to clusters.  
- **Clusters**: Define groups of destination servers and load-balancing policies.  

Refer to the `appsettings.json` file for detailed examples of route and cluster configurations.  
