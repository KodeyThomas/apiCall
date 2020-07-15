# apiCall

## Installation

```bash
git clone https://github.com/KodeyThomas/apiCall
```
Clone the repo into the tweak directory and add the following to each file

### Tweak.x
```objc
#import "apiCall/apiCall.h"
```
### MakeFile
```makefile
tweakName_FILES = *.x apiCall/apiCall.m
```

## Usage
```objc
// Call apiCall via sharedInstance
NSString *POSTurl = @"http://api.url"
NSString *params = @"yourAPIparamaters"
NSMutableDictionary *API_Response = [[apiCall sharedInstance] POST_JSON:POSTurl :params];

// The POST_JSON method is a POST request 'application/json' it returns a Dictionary you can handle
// based on the content
```

## Roadmap
Eventually, I am going to get around to finishing this library and adding XML types and GET requests
