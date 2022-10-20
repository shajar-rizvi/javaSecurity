# javaSecurity
When Cross error occor
* Just Add this in WebSecurityConfig
CorsConfiguration configuration = new CorsConfiguration();
configuration.applyPermitDefaultValues();
configuration.addAllowedMethod(HttpMethod.GET);
configuration.addAllowedMethod(HttpMethod.DELETE);
configuration.addAllowedMethod(HttpMethod.PUT);
configuration.addAllowedMethod(HttpMethod.OPTIONS);
http.cors().configurationSource(request -> configuration);
