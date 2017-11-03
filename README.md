# PHP-datetime-format

#### ตัวอย่าง 1/11/2017 14:38:08 จาก	timestamp	 2017-11-01 14:38:08
```php
$date = $row["updated_at"];
$date = date_create($date);
$date = date_format($date,"d/m/Y H:i:s");
