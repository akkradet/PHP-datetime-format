# PHP-datetime-format

#### ตัวอย่าง 1/11/2017 14:38:08 จาก	timestamp	 2017-11-01 14:38:08
```php
$date = $row["updated_at"];
$date = date_create($date);
$date = date_format($date,"d/m/Y H:i:s");

//Date
$thai_day_arr=array("อาทิตย์","จันทร์","อังคาร","พุธ","พฤหัสบดี","ศุกร์","เสาร์");
$thai_month_arr=array(
    "0"=>"",
    "1"=>"มกราคม",
    "2"=>"กุมภาพันธ์",
    "3"=>"มีนาคม",
    "4"=>"เมษายน",
    "5"=>"พฤษภาคม",
    "6"=>"มิถุนายน", 
    "7"=>"กรกฎาคม",
    "8"=>"สิงหาคม",
    "9"=>"กันยายน",
    "10"=>"ตุลาคม",
    "11"=>"พฤศจิกายน",
    "12"=>"ธันวาคม"                 
);

function thai_date($time){
    global $thai_day_arr,$thai_month_arr;
  
    $thai_date_return.= date("j",$time);
    $thai_date_return.= " " .$thai_month_arr[date("n",$time)];
    $thai_date_return.= " " .(date("Y",$time)+543);
    return $thai_date_return;
}
