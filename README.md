# surveygenerator

//FUNCTION ADDCSS
function addCss() {
    var cssText = "<style>.next{animation:animationFrames ease 1s;animation-iteration-count:1;transform-origin:50% 50%;animation-fill-mode:forwards;-webkit-animation:animationFrames ease 1s;-webkit-animation-iteration-count:1;-webkit-transform-origin:50% 50%;-webkit-animation-fill-mode:forwards;-moz-animation:animationFrames ease 1s;-moz-animation-iteration-count:1;-moz-transform-origin:50% 50%;-moz-animation-fill-mode:forwards;-o-animation:animationFrames ease 1s;-o-animation-iteration-count:1;-o-transform-origin:50% 50%;-o-animation-fill-mode:forwards;-ms-animation:animationFrames ease 1s;-ms-animation-iteration-count:1;-ms-transform-origin:50% 50%;-ms-animation-fill-mode:forwards}@keyframes animationFrames{0%{opacity:1;transform:translate(0,0)}20%{opacity:1;transform:translate(20px,0)}100%{opacity:0;transform:translate(-1000px,0)}}@-moz-keyframes animationFrames{0%{opacity:1;-moz-transform:translate(0,0)}20%{opacity:1;-moz-transform:translate(20px,0)}100%{opacity:0;-moz-transform:translate(-1000px,0)}}@-webkit-keyframes animationFrames{0%{opacity:1;-webkit-transform:translate(0,0)}20%{opacity:1;-webkit-transform:translate(20px,0)}100%{opacity:0;-webkit-transform:translate(-1000px,0)}}@-o-keyframes animationFrames{0%{opacity:1;-o-transform:translate(0,0)}20%{opacity:1;-o-transform:translate(20px,0)}100%{opacity:0;-o-transform:translate(-1000px,0)}}@-ms-keyframes animationFrames{0%,20%{opacity:1}0%{-ms-transform:translate(0,0)}20%{-ms-transform:translate(20px,0)}100%{opacity:0;-ms-transform:translate(-1000px,0)}}</style>";
    $(".imageBody").before(cssText);
    console.log("estoy en addCss");
}//END ADD CSS

//ONCLICK
 $(document).find(".steps td img").on('click', function() {
steps = steps+1;
console.log(steps);

 //$(this).closest( ".steps" ).css({"-webkit-transition":"transform 0.5s, opacity 0.3s", "transition":"transform 0.5s opacity 0.3s", "opacity":"0","transform":"translateY(-100%)","-webkit-transform":"translateY(-100%)","-moz-transform":"translateY(-100%)","-o-transform":"translateY(-100%)", "transition-timing-function":"easy", "transition-delay":".8s" });
 $(this).closest( ".steps" ).addClass( "next" );
/*
if(steps==lenghtSteps){
onclickContinue()
console.log("click");
}*/


  


});//END ON CLICK
