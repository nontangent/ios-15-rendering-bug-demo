# iOS 15 Rendering Bug Demo

## Bug Report
If the position of the body element is changed to `fixed`  when you scroll down and safari tool bar is collapsed,
the body element will be rerendered off about 85px down compared with the event position.

## Environment
- OS: iOS 15.2
- Device: iPad Pro
- Browser: Safari

## Demo
https://nontangent.github.io/ios-15-rendering-bug-demo/

## Reproduction
```sh
$ npx http-server
```

1. Access to http://localhost:8080 by your simulator.
2. Scroll down to `change body position fixed` and click it.
3. Click a green zone.
4. Confirm an alert with the message of `red zone is clicked`.