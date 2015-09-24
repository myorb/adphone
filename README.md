# adphone

#1  
Написать функцию преобразования строки, содержащей число в  
непосредственно число, не используя стандартные функции приведения типов  
(например “1252абв” в 1252)

  
#2  
Написать код приведения даты формата “01/18/2013 01:02:03”  
к формату “2013-01-18 01:02:03”  

#3  
Оптимизировать код и найти ошибку  

	$data = array(
		array('id'=>12345, 'topic' => 'text1', 'message' => 'text2'),
		array('id'=>23456, 'topic' => 'text3', 'message' => 'text4'),
		array('id'=>34567, 'topic' => 'text1', 'message' => 'text2'),
		...
	);
	foreach ($data as  $idx=>$row) {
		foreach ($data as $dbx=>$dbl)
		if ( $idx != $dbx && $dbl['topic'] == $row['topic'] && $dbl['message'] == $row['message'] )
		unset($data[$dbx])
	}
  
  
#4  
Написать абстрактный класс кеширования и одну реализацию на базе файлов  
или sqllite. Интерфейс класса:  

	interface I {
		public function put($key, $value, $expire = null);
		public function get($key);
	}
  


