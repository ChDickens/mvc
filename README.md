# mvc
// Convert variables e.g. {controller}
$route = preg_replace('/\{([a-z]+)\}/', '(?P<\1>[a-z-]+)', $route);

// Convert variables with custom regular expressions e.g. {id:\d+}
$route = preg_replace('/\{([a-z]+):([^\}]+)\}/', '(?P<\1>\2)', $route);
