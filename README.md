# iframe
1. Index HTML has Multiple iframes  
2. If iframes have xyz class ("I will add/remove the class from Index HTML, I will add/remove a class to anyone iframe") 
3. if the iframe has xyz class  only in that iframe make &lt;h2> red color 
4. if i remove xyz class from iframe make &lt;h2> normal back color  

My function inside iframe : 

    <script>
        $(function () {
            var iframes = parent.document.getElementsByTagName("iframe");
            console.log(iframes + ' iframe');
            for (var i = 0; i < iframes.length; i++) {
                var iframeGetAttribute = iframes[i].getAttribute("class");
                console.log(iframeGetAttribute + ' iframe GetAttribute');
                if (iframeGetAttribute == 'xyz') {
                    // ITS ALL WORKING FINE 
                }
            }
        });
    </script>
