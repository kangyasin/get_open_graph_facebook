# Get data facebook open graph OG

```markdown
<?php
function fetch_og($url)
{
    data = file_get_contents(url);
    $dom = new DomDocument;
    @$dom->loadHTML($data);
     
    $xpath = new DOMXPath($dom);
    query metatags dengan prefix og
    $metas = $xpath->query('//*/meta[starts-with(@property, \'og:\')]');

    $og = array();

    foreach($metas as $meta){
        # ambil nama properti tanpa menyertakan og
        $property = str_replace('og:', '', $meta->getAttribute('property'));
        # ambil konten dari properti tersebut
        $content = $meta->getAttribute('content');
        $og[$property] = $content;
    }

	return $og;
}
?>
```




## Cara penggunaan, cukup masukan url
```markdown
<?php

$og = fetch_og('http://www.kangyasin.com/2017/12/memilih-kamera-handphone-untuk-fotografi.html');

echo "<pre>";
print_r($og);
echo "</pre>";
echo "<hr>";

echo $og['title'];
echo "<hr>";

echo "<h1>Data Facebook Kangyasin.com</h1>";
echo "<h3>Link: <small><small>http://www.kangyasin.com/2017/12/memilih-kamera-handphone-untuk-fotografi.html</small></small></h3>";
foreach (og as $key => $value) {
    echo "<strong>key:</strong> ".$value;
    echo "<br>";
}

?>
```

