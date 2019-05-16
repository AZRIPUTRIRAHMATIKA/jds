# jds_azriputrirahmatika_jrbackend

<?php
class Palindrome
{
    public static function isPalindrome($data)
    {
      $datapali = $data;
      $tmp = strrev($datapali);
        $string_reverse = str_split($tmp);
        $$palindrome = '';
        
        foreach($string_reverse as $value){
          $palindrome.= $value;
        }
        print $palindrome;
        if($datapali == $palindrome){
          print "<br>Benar!! Itu Palindrome";
        } else {
          print "<br>Salah!! Bukan Palindrome";
        }
        return NULL;
    }
}

echo Palindrome::isPalindrome('kasurusak');
print"<br>";
echo Palindrome::isPalindrome('jeruk');
?>
