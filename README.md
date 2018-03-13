# jsnlib-export
匯出 CSV 

## 使用方式
````php
require_once '../vendor/autoload.php';

$result = \Jsnlib\Export::csv(new \Jsnlib\Ao(
[
    'TitleInfo' => ['編號', '姓名', '電話'],
    'ContentList' => 
    [
        ['1', '張先生', '0978-235-235'],
        ['4', '許小姐', '0978-233-111']
    ],
    'return_map' => true,
]));
````
### 輸出
````
"編號","姓名","電話" 
"1","張先生","0978-235-235" 
"4","許小姐","0978-233-111"
````
