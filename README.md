# Rotating--cube
....html.....
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>repl.it</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
    <div class="stage" style="width: 120px; height: 120px;">
<div class="cubespinner">
<div class="face1">1</div>
<div class="face2">2</div>
<div class="face3">3</div>
<div class="face4">4</div>
<div class="face5">5</div>
<div class="face6">6</div>
</div>
</div>
<style>
  .cubespinner{
    padding:180px
  }
    </style> 
  </body>
</html>
.....css......
<style type="text/css">

  @-webkit-keyframes spincube {
    from,to  { -webkit-transform: rotateX(0deg) rotateY(0deg) rotateZ(0deg); }
    16%      { -webkit-transform: rotateY(-90deg);                           }
    33%      { -webkit-transform: rotateY(-90deg) rotateZ(90deg);            }
    50%      { -webkit-transform: rotateY(-180deg) rotateZ(90deg);           }
    66%      { -webkit-transform: rotateY(-270deg) rotateX(90deg);           }
    83%      { -webkit-transform: rotateX(90deg);                            }
  }

  @keyframes spincube {
    from,to {
      -moz-transform: rotateX(0deg) rotateY(0deg) rotateZ(0deg);
      -ms-transform: rotateX(0deg) rotateY(0deg) rotateZ(0deg);
      transform: rotateX(0deg) rotateY(0deg) rotateZ(0deg);
    }
    16% {
      -moz-transform: rotateY(-90deg);
      -ms-transform: rotateY(-90deg);
      transform: rotateY(-90deg);
    }
    33% {
      -moz-transform: rotateY(-90deg) rotateZ(90deg);
      -ms-transform: rotateY(-90deg) rotateZ(90deg);
      transform: rotateY(-90deg) rotateZ(90deg);
    }
    50% {
      -moz-transform: rotateY(-180deg) rotateZ(90deg);
      -ms-transform: rotateY(-180deg) rotateZ(90deg);
      transform: rotateY(-180deg) rotateZ(90deg);
    }
    66% {
      -moz-transform: rotateY(-270deg) rotateX(90deg);
      -ms-transform: rotateY(-270deg) rotateX(90deg);
      transform: rotateY(-270deg) rotateX(90deg);
    }
    83% {
      -moz-transform: rotateX(90deg);
      -ms-transform: rotateX(90deg);
      transform: rotateX(90deg);
    }
  }

  .cubespinner {
    -webkit-animation-name: spincube;
    -webkit-animation-timing-function: ease-in-out;
    -webkit-animation-iteration-count: infinite;
    -webkit-animation-duration: 8s;

    animation-name: spincube;
    animation-timing-function: ease-in-out;
    animation-iteration-count: infinite;
    animation-duration: 8s;

    -webkit-transform-style: preserve-3d;
    -moz-transform-style: preserve-3d;
    -ms-transform-style: preserve-3d;
    transform-style: preserve-3d;

    -webkit-transform-origin: 60px 60px 0;
    -moz-transform-origin: 60px 60px 0;
    -ms-transform-origin: 60px 60px 0;
    transform-origin: 60px 60px 0;
  }

  .cubespinner div {
    position: absolute;
    width: 150px;
    height: 150px;
    border: 2px solid ash;
    background: rgba(124, 129, 101, 0.8);
    box-shadow: inset 0 0 0px white(0,0,0,0.2);
    line-height: 120px;
    text-align: center;
    font-size: 100px;
  }

  .cubespinner .face1 {
    -webkit-transform: translateZ(60px);
    -moz-transform: translateZ(60px);
    -ms-transform: translateZ(60px);
    transform: translateZ(60px);
  }
  .cubespinner .face2 {
    -webkit-transform: rotateY(90deg) translateZ(60px);
    -moz-transform: rotateY(90deg) translateZ(60px);
    -ms-transform: rotateY(90deg) translateZ(60px);
    transform: rotateY(90deg) translateZ(60px);
  }
  .cubespinner .face3 {
    -webkit-transform: rotateY(90deg) rotateX(90deg) translateZ(60px);
    -moz-transform: rotateY(90deg) rotateX(90deg) translateZ(60px);
    -ms-transform: rotateY(90deg) rotateX(90deg) translateZ(60px);
    transform: rotateY(90deg) rotateX(90deg) translateZ(60px);
  }
  .cubespinner .face4 {
    -webkit-transform: rotateY(180deg) rotateZ(90deg) translateZ(60px);
    -moz-transform: rotateY(180deg) rotateZ(90deg) translateZ(60px);
    -ms-transform: rotateY(180deg) rotateZ(90deg) translateZ(60px);
    transform: rotateY(180deg) rotateZ(90deg) translateZ(60px);
  }
  .cubespinner .face5 {
    -webkit-transform: rotateY(-90deg) rotateZ(90deg) translateZ(60px);
    -moz-transform: rotateY(-90deg) rotateZ(90deg) translateZ(60px);
    -ms-transform: rotateY(-90deg) rotateZ(90deg) translateZ(60px);
    transform: rotateY(-90deg) rotateZ(90deg) translateZ(60px);
  }
  .cubespinner .face6 {
    -webkit-transform: rotateX(-90deg) translateZ(60px);
    -moz-transform: rotateX(-90deg) translateZ(60px);
    -ms-transform: rotateX(-90deg) translateZ(60px);
    transform: rotateX(-90deg) translateZ(60px);
  }

</style>

<div class="stage" style="width: 150px; height: 150px;">
<div class="cubespinner">
<div class="face1">1</div>
<div class="face2">2</div>
<div class="face3">3</div>
<div class="face4">4</div>
<div class="face5">5</div>
<div class="face6">6</div>
</div>
</div>
