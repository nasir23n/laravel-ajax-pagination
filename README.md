# Laravel ajax pagination


## table structure
```$table->id();
$table->string('name');
$table->string('email');
$table->longText('description');
$table->timestamps();
```

## Controller Function

```
public function index() {
        $ajaxPagin = AjaxPagin::orderBy('id', 'ASC')->paginate(20);
        return $ajaxPagin;
}
 ```
