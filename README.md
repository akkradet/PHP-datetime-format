# PHP-datetime-format

$date = $row["updated_at"];
$date = date_create($date);
$date = date_format($date,"d/m/Y H:i:s");
