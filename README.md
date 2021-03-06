# kinesis-tail

`tail(1)` for Amazon Kinesis.

## Requirements

AWS Credentials should be configured under [AWS-SDK's standard location](https://blogs.aws.amazon.com/security/post/Tx3D6U6WSFGOK2H/A-New-and-Standardized-Way-to-Manage-Credentials-in-the-AWS-SDKs).

## Usage

List available streams.

```shell
$ AWS_REGION=ap-northeast-1 kinesis-tail
stream-foo
stream-bar
...

```

Tail specific stream.

```shell
$ AWS_REGION=ap-northeast-1 kinesis-tail stream-foo
foobarfoobar
```

Tail specific stream and shard.

```shell
$ AWS_REGION=ap-northeast-1 kinesis-tail stream-foo shardId-000000000002
foobarfoobar
```



# License
The MIT License (MIT)
Copyright (c) 2016 MinYoung Jung (http://kkung.net)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the “Software”), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
