# Leetcode - Two Sum 


```php
class Solution {
    function twoSum($nums, $target) {
        $new = [];
        foreach($nums as $i => $v){
            $find = $target - $v;
            if(isset($new[$find])) return [$new[$find], $i];
            $new[$v] = $i; 
        }
    }
}
```
