코드로 width 를 설정해 줄 때 분명히 self.view.frame.width 혹은 cell.view.frame.width 등으로 값을 줬음에도 불구하고 오른쪽이 잘리는 버그가 있었다.
![](20220609.png)

그럴 때 bounds.width 를 주면 꽉 차게 잘 들어가는 것을 알 수 있다.
왜 그런지는 파악해 봐야겠다.

storeWkWebviewMulti = WKWebView(frame: CGRect( x: 0, y: 0, width: view.bounds.width, height: webviewHeightPadding ), configuration: configuration )
