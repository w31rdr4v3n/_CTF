## Crypto

### A simple challenge

You can use [CyberChef](http://icyberchef.com) and decode it six times or use the base64 command to decode it.

```
base64 -d <<<"Vm0weE1HRXlTWGxVYTJoVllXeGFVMWx0ZEV0alZuQlhWbXQwYVUxVk5WZFpWVlUxWVZaS2RHUkVXbFpOYWtVd1dWUkdSbVF4VG5GUmJHaHBVakpvVVZkc1pEUmpNV1JIWTBWb2JGSnJTbTlXYkZaM1RVWmtXR1JIZEZOTmEzQXdWbTF3WVZaWFNuTlhiVVpoVmpOU1RGa3llRk5XTVd3MlVtMXNhVkl5WTNsV1Z6QXhaREZrVmsxWVJsWmhhelZvVld4YWNrMUdjRmhOVlhSclVteEtNVmxyWkRSWFJrcFdZa1JPVjFKc2NGUlZWRXBUVm0xS1IySkZOVk5TUlVVMQ==" | base64 -d | base64 -d | base64 -d | base64 -d | base64 -d
```

### Roman encryption 
```
Csddk Rtdetp,
Qcghb ykt jko ykto ptmmkoq,
Ykt igh tps qcep bsy qk osisevs ykto oswgou: jdgl{5ta5q1qtq10h_1p_b3y}
```
I used [quipqiup](https://www.quipqiup.com/) to decode it.

```
Hello Julius, Thank you for your support, You can use this key to receive your reward: flag{5um5t1tut10n_1s_k3y}
```

![quip image](/image/sample.png)

Change m by b in flag.

```
flag{5ub5t1tut10n_1s_k3y}
```

### Hextraordinary security

You can use [CyberChef](http://icyberchef.com) to decode the hex and find flag inside garbage with CTR+F or use xxd.

```
xxd -r -p <<<"hex_data_here" | grep flag
```
![Garbage image](/image/sample.png)



## Reverse

### You are not allowed 

I ran the executable to see how it works and that asks me a secret key.

![rev0 image](/image/sample.png)

So I used ltrace to see more clearly, functions called during execution.

![ltrace image](/image/sample.png)

As I have the secret key I restart the executable and I put it.

![flag_rev image](/image/sample.png)
