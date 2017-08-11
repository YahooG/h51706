# h51706
This is a demo for github


ssh出错 sign_and_send_pubkey: signing failed: agent refused operation
 Posted on 2016-05-26 |  Visitors 321
在服务器添加完公钥之后，ssh服务器然后报了这个错误

sign_and_send_pubkey: signing failed: agent refused operation
然后执行了以下命令才好。。

eval "$(ssh-agent -s)"
ssh-add

