# 阶乘N < 10000

#### 题目描述

给定一个数n，范围为0≤n≤100，请你编程精确的求出n的阶乘n！。

#### 输入

输入数据有多行，每行一个整数n，当n<0时输入结束。

#### 输出

输出n的阶乘。

#### 样例输入 [Copy](javascript:CopyToClipboard($('#sampleinput').text()))

```
1
2
3
4
-1
```

#### 样例输出 [Copy](javascript:CopyToClipboard($('#sampleoutput').text()))

```
1
2
6
24
```

```c++
#include<bits/stdc++.h>
using namespace std;
void solve(int n, string s) {
	int num = s.length();
	for (int i = 0; i < num; i++) {
		s[i] = (s[i] - 'a' + n) % 26 + 'a';
	}
	cout << s << "\n";
}
int main() {
	int n;
	string s;
	cin >> n;
	cin >> s;
	solve(n, s);
	return 0;
}
```

