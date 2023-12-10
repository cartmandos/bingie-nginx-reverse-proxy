# NGINX Reverse Proxy Server Configuration

## Functionality:

- Processes incoming requests and acts as a reverse proxy for multiple services.
- Directs traffic to the appropriate service based on the URL.
- Ensures security with SSL/TLS implementation and configuration.
- Manages caching for improved performance.
- Supported services include: Plex, Sonarr, Radarr, Ombi, Tautulli, Sabnzbd, NZBHydra, and the Plex web interface.

## Usage Notes:

- Modify the placeholder variable `$domain_name` to match your domain.
- Include SSL certificates for proper SSL/TLS functionality.

## Key Features:

- Secure SSL/TLS set-up and settings inc. session caching, stapling, protocols and ciphers.
- Automatic HTTP (port 80) to HTTPS (port 443) redirection to the corresponding URLs.
- Implemented optimizations and security measures like caching, GZIP compression, MIME types, and appropriate security headers.
- Handles PHP scripts using a dedicated FastCGI server (port 9000).
- Configures a dedicated location for serving the Plex web interface `(/plex/)`.
- Provides secure access for specific locations through an authentication request `(/auth-admin, /auth-user)`.
