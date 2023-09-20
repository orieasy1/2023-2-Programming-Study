<h3>스프링부트 시작하</h3>
스프링부트 프로젝트를 생성하기 위해서는 먼저 Create new Spring Starter Project를 눌러 프로젝트를 생성한다.
그리고 New Spring Starter Project Dependencies에서 꼭 Spring web을 클릭해 웹기능을 사용할 수 있도록 한다.

이후 HelloController라는 클래스를 만들어 아래와 같은 코드를 입력했는데

```java
package com.mysite.sbb;

import org.springframework.stereotype.Controller;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.ResponseBody;

@Controller
public class HelloController {
	@GetMapping("/hello")
	@ResponseBody
	public String hello() {
		return "Hello World!";
	}
}
```

