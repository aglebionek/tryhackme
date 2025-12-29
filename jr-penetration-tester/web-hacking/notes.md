1. Check /robots.txt for disallowed paths
2. Identify used technologies and frameworks
    - favicon hash:
    ```sh
    curl https://URL/.../favicon.ico | md5sum
    ```
    [Search for hash](https://owasp.org/www-community/favicons_database)
    - HTTP headers analysis
    ```sh
    curl -I https://URL
    ```
3. Check sitemap.xml for structure