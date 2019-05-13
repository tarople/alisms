## 阿里云短信发送，参照于PHP版本

示例代码
````
    ak := "ak"
    sk := "sk"
    
    result, err := alisms.New(ak, sk).
        Request("手机号码", "短信签名", "模板code", "{\"code\":\"1234\"}")
    
    if err != nil {
        log.Fatalln(err)
    }

    fmt.Println(result)
````
