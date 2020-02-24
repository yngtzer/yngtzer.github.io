---
layout: post
title: "Spring Mock Mvc"
date: 2020-02-23  23:22:00 +0800
categories: spring mockmvc
---

## Using Spring MockMvc for API Testing

        @WebMvcTest(GreetingController.class)
        public class WebMockTest {

            @Autowired
            private MockMvc mockMvc;

            @MockBean
            private GreetingService service;

            @Test
            public void greetingShouldReturnMessageFromService() throws Exception {
                when(service.greet()).thenReturn("Hello, Mock");
                this.mockMvc.perform(get("/greeting"))
                    .andDo(print())
                    .andExpect(status().isOk())
                    .andExpect(content().string(containsString("Hello, Mock")));
            }
        }

Reference [MockMvcResultMatchers](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/test/web/servlet/result/MockMvcResultMatchers.html) for all available method in "andExpect"