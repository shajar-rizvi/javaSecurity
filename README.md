# javaSecurity
When Cross error occor
* When frontend try to access and landed on you cors this will right access to the request . Just add this  
# In WebSecurityConfig
* CorsConfiguration configuration = new CorsConfiguration();
* configuration.applyPermitDefaultValues();
* configuration.addAllowedMethod(HttpMethod.GET);
* configuration.addAllowedMethod(HttpMethod.DELETE);
* configuration.addAllowedMethod(HttpMethod.PUT);
* configuration.addAllowedMethod(HttpMethod.OPTIONS);
* http.cors().configurationSource(request -> configuration);
