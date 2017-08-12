# h51706
This is a demo for github


ssh出错 sign_and_send_pubkey: signing failed: agent refused operation
 Posted on 2016-05-26 |  Visitors 321
在服务器添加完公钥之后，ssh服务器然后报了这个错误

sign_and_send_pubkey: signing failed: agent refused operation
然后执行了以下命令才好。。

eval "$(ssh-agent -s)"
ssh-add



from django.shortcuts import get_object_or_404 
product = get_object_or_404(Product, pk=1) 
Product是要查询的model,后面的pk＝1是查询条件，你可以根据你需要查询的情况来写条件。 上面的例子也可以写成下面这样的形式：

from django.http import Http404

try:
    product = Product.objects.get(pk=1)
except MyModel.DoesNotExist:
    raise Http404
看来用django get_object_or_404方法可以省下你很多操作，有兴趣可以看看django.shortcuts 模块包里面的其他的方法， 会让你能够在提高编程的效率。
