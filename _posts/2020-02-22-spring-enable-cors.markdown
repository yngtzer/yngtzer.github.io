---
layout: post
title:  "Enable Spring CORS"
date:   2020-02-22 23:26:00 +0800
categories: spring cors
---

## Enable Spring CORS

1. Class/Controller Level

        @CrossOrigin(origins = "*", allowedHeaders = "*")
        @Controller
        public class HomeController {
            @GetMapping("/")
            public String getHome(Model model) {
                return "home";
            }
        }

2. Method Level

        @Controller
        public class HomeController {
            @CrossOrigin(origins = "*", allowedHeaders = "*")
            @GetMapping("/")
            public String getHome(Model model) {
                return "home";
            }
        }

3. Global Level, using WebMvcConfigurer Bean
    
        @Configuration
        public class CorsConfiguration 
        {
            @Bean
            public WebMvcConfigurer corsConfigurer() 
            {
                return new WebMvcConfigurer() {
                    @Override
                    public void addCorsMappings(CorsRegistry registry) {
                        registry.addMapping("/**").allowedOrigins("http://localhost:8080");
                    }
                };
            }
        }