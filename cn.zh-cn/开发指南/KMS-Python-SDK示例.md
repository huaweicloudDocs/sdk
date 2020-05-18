# KMS Python SDK示例<a name="sdk_02_0027"></a>

密钥管理服务，即KMS（Key Management Service），是一种安全、可靠、简单易用的密钥托管服务，帮助用户集中管理密钥，保护密钥安全。

KMS通过使用硬件安全模块HSM（Hardware Security Module）保护密钥安全，帮助用户轻松创建和管理密钥，所有的用户密钥都由HSM中的根密钥保护，避免密钥泄露。KMS对密钥的所有操作都会进行访问控制及日志跟踪，提供所有密钥的使用记录，满足审计和合规性要求。

## 创建用户主密钥<a name="section10673294192958"></a>

您可以根据以下代码，使用Python OpenStack SDK创建一条用户主密钥。

```
 def create_key(conn):
    key_dict = {
        "key_alias": "test-key-123-456789223", "realm": "123"       
    }
    key = conn.kms.create_key(**key_dict) 
```

## 启用密钥<a name="section31982478192958"></a>

您可以根据以下代码，启用一条已经禁用的密钥。

```
def enable_key(conn, key):
    # a string of key id or an object of Key
    print(conn.kms.enable_key(key))   
```

## 创建数据密钥<a name="section60390938"></a>

您可以根据以下代码，创建一条数据密钥。

```
def create_data_key(conn, key):      
    data_key_dict={
    "datakey_length":"512"
    }
    print(conn.kms.create_datakey(key, **data_key_dict))
```

## 加密数据密钥<a name="section59952153194055"></a>

您可以根据以下代码，加密已创建的数据密钥，其中，plain\_text的值应为创建数据密钥接口返回。

```
def encrypt_datakey(conn, key):
    params = {
        "plain_text": "4c5062132d3b1b450d1aff4cd49bb828c09e602e3678b3c8d9be5429fa22be17439a1c7bd167e76d1be8f0cadda76940c98e4483bc32312534ce98db824329eb
",
        "datakey_plain_length": "64"
    }
    datakey = conn.kms.encrypt_datakey(key, **params)
    print(datakey)
```

