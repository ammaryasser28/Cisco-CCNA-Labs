## Commands

```bash
# الدخول للتهيئة على كل راوتر
R1> enable
R1# configure terminal
R2> enable
R2# configure terminal

# ضبط Enable Password
R1(config)# enable password cisco
R2(config)# enable password cisco

# التحقق قبل التشفير
R1# show running-config
R2# show running-config

# تفعيل تشفير الباسوردات
R1(config)# service password-encryption
R2(config)# service password-encryption

# التحقق بعد التشفير
R1# show running-config
R2# show running-config

# تعطيل تشفير الباسوردات
R1(config)# no service password-encryption
R2(config)# no service password-encryption

# التحقق بعد الإيقاف
R1# show running-config
R2# show running-config

# حفظ التهيئة
R1# write memory
R2# write memory


---

## **2️⃣ تنسيق شرح الأوامر**
- استخدم جدول Markdown لوصف كل أمر ووظيفته:

```markdown
## Commands Explanation

| Command | Function | Notes |
|---------|---------|-------|
| enable password cisco | ضبط الباسورد للدخول لوضع Privileged Exec | يظهر واضح قبل التشفير |
| service password-encryption | تشفير كل الباسوردات النصية | Enable Password يظهر مشفر بعد التفعيل |
| no service password-encryption | إيقاف تشفير الباسوردات | Enable Password يظهر واضح مرة أخرى |
