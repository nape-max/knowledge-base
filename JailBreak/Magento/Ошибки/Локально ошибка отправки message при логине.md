Нужно отключить модуль Двухфакторной аутентификации в Magento:
```bash
bin/magento module:disable Magento_TwoFactorAuth \
&& bin/magento c:f
```
