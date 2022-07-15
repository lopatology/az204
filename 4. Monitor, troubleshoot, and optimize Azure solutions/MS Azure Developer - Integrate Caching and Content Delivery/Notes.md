1. Configuring cache and Expiration policies in azure CDN
   Create CDNs with "Front Door and CDN profiles"

2. Configuring cache and expiration poplicies for Azure Redis Cache
   Create "Azure Cache for Redis" resource

3. Implementing Application caching patterns:
   Pattrens:

   - Cache-aside Pattern
   - Content Cache Pattern
   - User session caching pattern
   - Advanced patterns:
     - job and message queuing
     - distributed transactions

   Estimating Cache size
   a. Number of current cached objects
   b. Size of cached objects
   c. Number of cache requests
   d. Cache expiration policy

   Redis-CLI has special tool named "Redis-benchmark" witch can simulate load on Redis cache instance:
   Redis-benchmark -q -n 10000

   Tool cannot be run from AzurePortal. Although we can create VM that contains Redis CLI

   Securing Redis Cache:
   a. Encript in Transit:

   - Use TLS 1.2
   - TLS 1.1 supported for compatibility
   - HTTP connections disabled by default

   b. Encription at Rest:

   - In memory data is not encripted
   - In premium tiers - we have data persistance. Data persistance is encrypted
