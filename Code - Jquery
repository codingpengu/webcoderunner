<script type="text/javascript">
            function updateOut(){
                $("iframe").contents().find("html").html("<html><head><style type='text/css'>" + $("#csspanel").val() + "</style></head><body>" + $("#htmlpanel").val() + "</body></html>");
                document.getElementById("outputpanel").contentWindow.eval($("#jspanel").val());
            }
            $(".togglebutton").hover(function() {
                $(this).addClass("highlighted");
            },function(){
                $(this).removeClass("highlighted");
            });
            $(".togglebutton").click(function(){
                $(this).toggleClass("active");
                $(this).removeClass("highlighted");
                var panelid = $(this).attr("id") + "panel";
                $("#"+panelid).toggleClass("hidden");
                var numberofacivepanels =4 - $('.hidden').length;
                $(".panel").width(($(window).width()/numberofacivepanels)-10);
            });
            $(".panel").height($(window).height()-$("#topbar").height()-15);
            $(".panel").width(($(window).width()/2)-10);
            updateOut();
            $("textarea").on('change keyup paste',function(){
                updateOut();   
            });
            $(".panel").hover(function(){
                $(this).toggleClass("touch");
            });    
       
            $("textarea").attr('spellcheck', false);
    

        </script>
 
