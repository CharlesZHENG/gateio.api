# gateio.api
Gate.io API 的C#实现

## 使用 GateIO.API

所有的方法在API类中，使用前先调用

```
   static void Main(string[] args)
   {
     API.SetKey(key,secret);
     //var balance = API.GetBalancesAsync().GetAwaiter().GetResult();
     var marketDeep= API.OrderBookAsync("iht","usdt").GetAwaiter().GetResult();     
     Console.Read();
   }
```

设置密钥

然后调用相应的方法即可，代码中都有注释。