# Big_File
基于Webuploader插件的大文件分片上传

# 原理
使用Webuploader将大文件拆分为片，减少一次传输的压力和避免各种问题导致的失败。
上传完成后由后台进行整合，保证文件可以正常传输。

# 难点
目前本地环境测试,2G的文件是正常的。

由于没有更大的测试，猜想会发生问题的情况

php 如果一个文件的分片太多，脚本的执行时间很很长，必须保证完全合并

检查每一个分片的正确性

错误机制，分片上传失败之后重新上传

以上是感觉可能会发生错误的情况，具体需要测试才能一步步解决
