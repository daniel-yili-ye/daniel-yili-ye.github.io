+++
title = "Testing Code Snippets"
date = "2025-05-31"
tags = ["test", "code"]
draft = false
+++

# Code Snippet Testing

Let's test different types of code snippets to make sure they render correctly.

## Inline Code

Here's some `inline code` in a sentence. You can also use `const variable = "value"` inline.

## JavaScript

```javascript
function greetUser(name) {
  const greeting = `Hello, ${name}!`;
  console.log(greeting);
  return greeting;
}

// Usage
const user = "Daniel";
greetUser(user);
```

## Python

```python
def calculate_fibonacci(n):
    """Calculate the nth Fibonacci number."""
    if n <= 1:
        return n
    return calculate_fibonacci(n-1) + calculate_fibonacci(n-2)

# Example usage
for i in range(10):
    print(f"fib({i}) = {calculate_fibonacci(i)}")
```

## CSS

```css
.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
}

.title {
  font-family: 'Inter', sans-serif;
  color: #333;
  font-size: 2rem;
}
```

## Bash/Shell

```bash
#!/bin/bash

# Install Hugo
brew install hugo

# Create new site
hugo new site myblog
cd myblog

# Add theme
git submodule add https://github.com/janraasch/hugo-bearblog.git themes/hugo-bearblog
```

## HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Blog</title>
</head>
<body>
    <h1>Welcome to my blog!</h1>
    <p>This is a test page.</p>
</body>
</html>
```

## YAML (Hugo Config)

```yaml
baseURL: 'https://example.com'
languageCode: 'en-us'
title: 'My Hugo Blog'
theme: 'hugo-bearblog'

params:
  description: 'A test blog'
  
markup:
  highlight:
    style: 'github'
    lineNos: false
```

## Code Without Language

```
This is a plain code block
without any specific language
highlighting. It should still
use monospace font.
``` 