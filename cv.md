# Aliaksandr Fiarsovich
**Date of birth:** 26/11/1982
**Gender:** Male
**Nationality:** Belarusian

## Contacts
**Email address:** [7916884@gmail.com](mailto:7916884@gmail.com)

## Work experience
* **Web programmer**
  Center for implementation of scientific and technical developments
  14/02/2005  – 31/07/2007
  Brest, Belarus
  Website development and support ([brest-region.gov.by](http://brest-region.gov.by), [tric.info](http://tric.info/en/)). Digital infrastructure support.

* **Web programmer**
  Regional newspaper "Vecherniy Brest"
  03/09/2007  – 02/09/2014
  Brest, Belarus
  Website development and support ([vb.by](https://vb.by)). Digital infrastructure support. Newspaper layout (Adobe InDesign).

* **Web programmer**
  [priminer.eu](http://priminer.eu), [motoplanet.by](https://motoplanet.by), [dostavka24.pl](https://dostavka24.pl), [moto-planet.ru](https://moto-planet.ru), [kakest.by](https://www.kakest.by), [holodgrodno.by](https://holodgrodno.by), [remontholod.by](https://remontholod.by), [vending.by](https://vending.by)
  03/10/2014  – Current
  Grodno, Belarus
  Website development and support.

## Education

* **Brest State Technical University**
* Engineer in Information Technologies
  01/09/2000  – 30/06/2005
  267 Moskovskaya str., Brest, Belarus

## Language skills

#### Mother tongue(s)
* Russian
* Belarusian

#### Other language(s)
* English (B2)
* Polish (B2)

## Skills

### Programming languages

* PHP
* SQL
*  jQuery
* JavaScript
* HTML 5
* Ajax
* CSS (SASS LESS)

### Code example

```
class mail
{
    static $data_charset = 'UTF-8';
    static $send_charset = 'UTF-8';
    static $name = 'test.bypl';
    static $email = 'info@dostavka24.pl';

    static function mime_header_encode($str)
    {
        if (self::$data_charset != self::$send_charset) {
            $str = iconv(self::$data_charset, self::$send_charset, $str);
        }
        return '=?' . self::$send_charset . '?B?' . base64_encode($str) . '?=';
    }

    static function send(
        $email_to,
        $subject,
        $body,
        $html = FALSE
    )
    {
        $to = $email_to;
        $subject = self::mime_header_encode($subject);
        $from = self::mime_header_encode(self::$name) . ' <' . self::$email . '>';
        if (self::$data_charset != self::$send_charset) {
            $body = iconv(self::$data_charset, self::$send_charset, $body);
        }
        $headers = "From: $from\r\n";
        $type = ($html) ? 'html' : 'plain';
        $headers .= "Content-type: text/$type; charset=" . self::$send_charset . "\r\n";
        $headers .= "Mime-Version: 1.0\r\n";
        return mail($to, $subject, $body, $headers);
    }
}
```

### Web development

* phpStorm
* MySQL
* Unix Linux und Unix Shell
* Git
* Apache
* Nginx
* Adobe Dreamwaver
* Adobe Photoshop
* Google Analytics
* WordPress

### Operating Systems

* Windows
* Mac OS
* Linux
* iOS

### Office programs

* Microsoft Word
* Microsoft Exel
* Microsoft PowerPoint
