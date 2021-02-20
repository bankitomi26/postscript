<!DOCTYPE html>
<!-- saved from url=(0050)http://timbaumann.info/svd-image-compression-demo/ -->
<html><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
  
  <title>SVD-Demo: Image Compression</title>
  <link rel="shortcut icon" type="image/png" href="http://timbaumann.info/svd-image-compression-demo/favicon.png">
  <link rel="stylesheet" href="./SVD-Demo_ Image Compression_files/nouislider.min.css">
  <link rel="stylesheet" href="./SVD-Demo_ Image Compression_files/slick.css">
  <link rel="stylesheet" href="./SVD-Demo_ Image Compression_files/slick-theme.css">
  <link rel="stylesheet" href="./SVD-Demo_ Image Compression_files/style.css">
</head>

<body>
  <div class="wrapper">
    <h1>
      Image Compression with<br>
      Singular Value Decomposition
    </h1>
    <noscript>The interactive demo runs purely on the client-side. You therefore have to enable JavaScript to enjoy it.</noscript>
  </div>

  <div class="app" id="app"><div><div class="image-container" style="width: 840px; height: 382px;"><img width="600" height="402" src="./SVD-Demo_ Image Compression_files/img/1.jpg"><p class="info-bar"><span>Please wait …</span></p><div class="stats" style="left: 620px;"><table><tbody><tr><th class="label">Image size</th><td>600 × 402</td></tr><tr><th class="label">#pixels</th><td>= 241200</td></tr></tbody></table><p><span class="label">Uncompressed size</span><br>proportional to number of pixels</p><p><span class="label">Compressed size</span><br>approximately proportional to <br>402 × 5 + 5 + 5 × 600 <br>= 5015</p><p><span class="label">Compression ratio</span><br>241200 / 5015 = 48.10</p><p><a class="button toggle-show-svs " href="http://timbaumann.info/svd-image-compression-demo/#">Show singular values</a></p><p class="hint"><a class="toggle-hover-original active" href="http://timbaumann.info/svd-image-compression-demo/#"><span class="check-box"><span>☑</span></span><span class="text">hover to see the original picture</span></a></p></div></div><div class="wrapper"><div class="options"><div class="slider noUi-target noUi-ltr noUi-horizontal noUi-txt-dir-ltr"><div class="noUi-base"><div class="noUi-connects"></div><div class="noUi-origin" style="transform: translate(-920%, 0px); z-index: 4;"><div class="noUi-handle noUi-handle-lower" data-handle="0" tabindex="0" role="slider" aria-orientation="horizontal" aria-valuemin="1.0" aria-valuemax="402.0" aria-valuenow="5.0" aria-valuetext="5.00"><div class="noUi-touch-area"></div></div></div></div><div class="noUi-pips noUi-pips-horizontal"><div class="noUi-marker noUi-marker-horizontal noUi-marker-large" style="left: 0%;"></div><div class="noUi-value noUi-value-horizontal noUi-value-large" data-value="1" style="left: 0%;">1</div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 2%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 4%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 6%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 8%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 10%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 12%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 14%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 16%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 18%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 19.2%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 20.4%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 21.6%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 22.8%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 24%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 25.2%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 26.4%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 27.6%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 28.8%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 30%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 31.125%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 32.25%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 33.375%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 34.5%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 35.625%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 36.75%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 37.875%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 39%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 40.125%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 41.25%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 42.375%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 43.5%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 44.625%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 45.75%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 46.875%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 48%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 49.7219%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 51.4437%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 53.1656%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 54.8874%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 56.6093%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 58.3311%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 60.053%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 61.7748%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 63.4967%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 65.2185%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 66.9404%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 68.6623%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 70.3841%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 72.106%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 73.8278%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 75.5497%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 77.2715%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 78.9934%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 80.7152%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 82.4371%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 84.1589%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 85.8808%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 87.6026%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 89.3245%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 91.0464%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 92.7682%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 94.4901%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 96.2119%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 97.9338%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 99.6556%;"></div><div class="noUi-marker noUi-marker-horizontal noUi-marker-normal" style="left: 100%;"></div></div></div></div><p>Change the number of singular values using the slider. Click on one of these images to compress it:</p><div class="slick-slider gallery slick-initialized" dir="ltr"><button type="button" data-role="none" class="slick-arrow slick-prev slick-disabled" style="display: block;"> Previous</button><div class="slick-list"><div class="slick-track" style="width: 2400px; opacity: 1; transform: translate3d(0px, 0px, 0px);"><div data-index="0" class="slick-slide slick-active slick-current" tabindex="-1" aria-hidden="false" style="outline: none; width: 160px;"><div><div class="image" tabindex="-1" style="width: 100%; display: inline-block;"><a href="http://timbaumann.info/svd-image-compression-demo/example-images/cats_medium.jpg"><img width="150" height="150" src="./SVD-Demo_ Image Compression_files/cats_small.jpg"></a><p class="caption"><a href="https://www.flickr.com/photos/jetske/5827857531/">By Jetske</a></p></div></div></div><div data-index="1" class="slick-slide slick-active" tabindex="-1" aria-hidden="false" style="outline: none; width: 160px;"><div><div class="image" tabindex="-1" style="width: 100%; display: inline-block;"><a href="http://timbaumann.info/svd-image-compression-demo/example-images/tree_medium.jpg"><img width="150" height="150" src="./SVD-Demo_ Image Compression_files/tree_small.jpg"></a><p class="caption"><a href="https://www.flickr.com/photos/aigle_dore/15061080128/">By Moyan Brenn</a></p></div></div></div><div data-index="2" class="slick-slide slick-active" tabindex="-1" aria-hidden="false" style="outline: none; width: 160px;"><div><div class="image" tabindex="-1" style="width: 100%; display: inline-block;"><a href="http://timbaumann.info/svd-image-compression-demo/example-images/mondrian_medium.jpg"><img width="150" height="150" src="./SVD-Demo_ Image Compression_files/mondrian_small.jpg"></a><p class="caption"><a href="https://www.flickr.com/photos/raelga/4408707212/">By Rael Garcia Arnes</a></p></div></div></div><div data-index="3" class="slick-slide slick-active" tabindex="-1" aria-hidden="false" style="outline: none; width: 160px;"><div><div class="image" tabindex="-1" style="width: 100%; display: inline-block;"><a href="http://timbaumann.info/svd-image-compression-demo/example-images/nyc_medium.jpg"><img width="150" height="150" src="./SVD-Demo_ Image Compression_files/nyc_small.jpg"></a><p class="caption"><a href="https://www.flickr.com/photos/isherwoodchris/3096255994/">By Chris Isherwood</a></p></div></div></div><div data-index="4" class="slick-slide slick-active" tabindex="-1" aria-hidden="false" style="outline: none; width: 160px;"><div><div class="image" tabindex="-1" style="width: 100%; display: inline-block;"><a href="http://timbaumann.info/svd-image-compression-demo/example-images/girl_medium.jpg"><img width="150" height="150" src="./SVD-Demo_ Image Compression_files/girl_small.jpg"></a><p class="caption"><a href="https://www.flickr.com/photos/25228175@N08/5896000539/">By Elvin</a></p></div></div></div><div data-index="5" class="slick-slide" tabindex="-1" aria-hidden="true" style="outline: none; width: 160px;"><div><div class="image" tabindex="-1" style="width: 100%; display: inline-block;"><a href="http://timbaumann.info/svd-image-compression-demo/example-images/royal_stewart_medium.jpg"><img width="150" height="150" src="./SVD-Demo_ Image Compression_files/royal_stewart_small.jpg"></a><p class="caption"><a href="https://en.wikipedia.org/wiki/Royal_Stewart_tartan">The Royal Stewart tartan</a></p></div></div></div><div data-index="6" class="slick-slide" tabindex="-1" aria-hidden="true" style="outline: none; width: 160px;"><div><div class="image" tabindex="-1" style="width: 100%; display: inline-block;"><a href="http://timbaumann.info/svd-image-compression-demo/example-images/randbitmap-rdo_medium.png"><img width="150" height="150" src="./SVD-Demo_ Image Compression_files/randbitmap-rdo_small.png"></a><p class="caption"><a href="https://www.random.org/bitmaps/">Random data</a></p></div></div></div><div data-index="7" class="slick-slide" tabindex="-1" aria-hidden="true" style="outline: none; width: 160px;"><div><div class="image" tabindex="-1" style="width: 100%; display: inline-block;"><a href="http://timbaumann.info/svd-image-compression-demo/example-images/girih_pattern_medium.jpg"><img width="150" height="150" src="./SVD-Demo_ Image Compression_files/girih_pattern_small.jpg"></a><p class="caption"><a href="https://en.wikipedia.org/wiki/Girih#/media/File:Samarkand_Shah-i_Zinda_Tuman_Aqa_complex_cropped2.jpg">Girih pattern by İnfoCan</a></p></div></div></div><div data-index="8" class="slick-slide" tabindex="-1" aria-hidden="true" style="outline: none; width: 160px;"><div><div class="image" tabindex="-1" style="width: 100%; display: inline-block;"><a href="http://timbaumann.info/svd-image-compression-demo/example-images/keep-calm-and-use-svd_medium.png"><img width="150" height="150" src="./SVD-Demo_ Image Compression_files/keep-calm-and-use-svd_small.png"></a><p class="caption"><a href="http://www.keepcalm-o-matic.co.uk/">Made with the KC-O-M</a></p></div></div></div><div data-index="9" class="slick-slide" tabindex="-1" aria-hidden="true" style="outline: none; width: 160px;"><div><div class="image" tabindex="-1" style="width: 100%; display: inline-block;"><a href="http://timbaumann.info/svd-image-compression-demo/example-images/skater_boy_medium.jpg"><img width="150" height="150" src="./SVD-Demo_ Image Compression_files/skater_boy_small.jpg"></a><p class="caption"><a href="https://flic.kr/p/keMZvg">By Chris Goldberg</a></p></div></div></div><div data-index="10" class="slick-slide" tabindex="-1" aria-hidden="true" style="outline: none; width: 160px;"><div><div class="image" tabindex="-1" style="width: 100%; display: inline-block;"><a href="http://timbaumann.info/svd-image-compression-demo/example-images/quiz1_medium.jpg"><img width="150" height="150" src="./SVD-Demo_ Image Compression_files/question_mark_small.jpg"></a><p class="caption"><a href="https://flic.kr/p/4bpEpb">By Francisco Martins</a></p></div></div></div><div data-index="11" class="slick-slide" tabindex="-1" aria-hidden="true" style="outline: none; width: 160px;"><div><div class="image" tabindex="-1" style="width: 100%; display: inline-block;"><a href="http://timbaumann.info/svd-image-compression-demo/example-images/quiz2_medium.jpg"><img width="150" height="150" src="./SVD-Demo_ Image Compression_files/question_mark_small.jpg"></a><p class="caption"><a href="https://flic.kr/p/5yWPDc">By Eleonora Gorini</a></p></div></div></div><div data-index="12" class="slick-slide" tabindex="-1" aria-hidden="true" style="outline: none; width: 160px;"><div><div class="image" tabindex="-1" style="width: 100%; display: inline-block;"><a href="http://timbaumann.info/svd-image-compression-demo/example-images/quiz3_medium.jpg"><img width="150" height="150" src="./SVD-Demo_ Image Compression_files/question_mark_small.jpg"></a><p class="caption"><a href="https://flic.kr/p/enTNR5">By melfoody</a></p></div></div></div><div data-index="13" class="slick-slide" tabindex="-1" aria-hidden="true" style="outline: none; width: 160px;"><div><div class="image" tabindex="-1" style="width: 100%; display: inline-block;"><a href="http://timbaumann.info/svd-image-compression-demo/example-images/quiz4_medium.jpg"><img width="150" height="150" src="./SVD-Demo_ Image Compression_files/question_mark_small.jpg"></a><p class="caption"><a href="https://goo.gl/oH2BLt">By VvG</a></p></div></div></div><div data-index="14" class="slick-slide" tabindex="-1" aria-hidden="true" style="outline: none; width: 160px;"><div><div class="image" tabindex="-1" style="width: 100%; display: inline-block;"><a href="http://timbaumann.info/svd-image-compression-demo/example-images/quiz5_medium.jpg"><img width="150" height="150" src="./SVD-Demo_ Image Compression_files/question_mark_small.jpg"></a><p class="caption"><a href="https://flic.kr/p/7TdBUA">By Sergiu Bacioiu</a></p></div></div></div></div></div><button type="button" data-role="none" class="slick-arrow slick-next" style="display: block;"> Next</button></div><p><span class="valign">You can compress your own images by using the</span><span class="button file-input-button"><span>file picker</span><input type="file" accept="image/*" class="file-input"></span><span class="valign">or by dropping them on this page.</span></p></div></div></div>

  <div class="wrapper">
    <div class="explanation clearfix">
      <div class="left-column">
        <h2>About Singular Value Decomposition</h2>
        <p>
          A matrix of size <span class="math">m × n</span> is a grid of real numbers consisting of <span class="math">m</span> rows and <span class="math">n</span> columns.
          In linear algebra, a branch of mathematics, matrices of size <span class="math">m × n</span> describe linear mappings from <span class="math">n</span>-dimensional to <span class="math">m</span>-dimensional space.
          The word linear roughly means that straight lines map to straight lines and the origin in <span class="math">n</span>‑dimensional space maps to the origin in <span class="math">m</span>‑dimensional space.
          When we have an <span class="math">(m × n)</span>‑matrix <span class="math">A</span> and a <span class="math">(n × k)</span>‑matrix <span class="math">B</span>, we can compute the product <span class="math">AB</span> which is an <span class="math">(m × k)</span>‑matrix.
          The mapping corresponding to <span class="math">AB</span> is exactly the composition of the mappings corresponding to <span class="math">A</span> and <span class="math">B</span> respectively.
        </p>
        <p>
          <a href="https://en.wikipedia.org/wiki/Singular_value_decomposition">Singular Value Decomposition</a> (SVD) states that every <span class="math">(m × n)</span>‑matrix <span class="math">A</span> can be written as a product
        </p>
        <div class="schema schema-a">
          <div class="matrix matrix-a">
            <div class="rows">m</div>
            <div class="cols">n</div>
            A
          </div>
          <div class="equals">=</div>
          <div class="matrix matrix-u">
            <div class="rows">m</div>
            <div class="cols">m</div>
            U
          </div>
          <div class="mult-dot mult-dot-1"></div>
          <div class="matrix matrix-sigma">
            <div class="rows">m</div>
            <div class="cols">n</div>
            <div class="sv" style="left: 0px; top: 0px;"></div>
            <div class="sv" style="left: 5px; top: 5px;"></div>
            <div class="sv" style="left: 10px; top: 10px;"></div>
            <div class="sv" style="left: 15px; top: 15px;"></div>
            <div class="sv" style="left: 20px; top: 20px;"></div>
            <div class="sv" style="left: 25px; top: 25px;"></div>
            <div class="sv" style="left: 30px; top: 30px;"></div>
            <div class="sv" style="left: 35px; top: 35px;"></div>
            <div class="sv" style="left: 40px; top: 40px;"></div>
            <div class="sv" style="left: 45px; top: 45px;"></div>
            Σ&nbsp;&nbsp;
          </div>
          <div class="mult-dot mult-dot-2"></div>
          <div class="matrix matrix-v">
            <div class="rows">n</div>
            <div class="cols">n</div>
            V <sup style="font-size: 0.7em;">T</sup>
          </div>
        </div>
        <p>
          where <span class="math">U</span> and <span class="math">V</span> are orthogonal matrices and the the matrix <span class="math">Σ</span> consists of descending non-negative values on its diagonal and zeros elsewhere.
          The entries <span class="math">σ<sub>1</sub> ≥ σ<sub>2</sub> ≥ σ<sub>3</sub> ≥ … ≥ 0</span> on the diagonal of <span class="math">Σ</span> are called the <em>singular values</em> (SVs) of <span class="math">A</span>.
          Geometrically, <span class="math">Σ</span> maps the <span class="math">j</span>‑th unit coordinate vector of <span class="math">n</span>‑dimensional space to the <span class="math">j</span>‑th coordinate vector of <span class="math">m</span>‑dimensional space, scaled by the factor <span class="math">σ<sub>j</sub></span>.
          Orthogonality of <span class="math">U</span> and <span class="math">V</span> means that they correspond to rotations (possibly followed by a reflection) of <span class="math">m</span>‑dimensional and <span class="math">n</span>‑dimensional space respectively.
          Therefore only <span class="math">Σ</span> changes the length of vectors.
        </p>
        <h2>Using SVD for image compression</h2>
        <p>
          We can decompose a given image into the three color channels red, green and blue.
          Each channel can be represented as a <span class="math">(m × n)</span>‑matrix with values ranging from 0 to 255.
          We will now compress the matrix <span class="math">A</span> representing one of the channels.
        </p>
        <p>
          To do this, we compute an approximation to the matrix <span class="math">A</span> that takes only a fraction of the space to store.
          Now here's the great thing about SVD: the data in the matrices <span class="math">U</span>, <span class="math">Σ</span> and <span class="math">V</span> is sorted by how much it contributes to the matrix <span class="math">A</span> in the product.
          That enables us to get quite a good approximation by simply using only the most important parts of the matrices.
        </p>
      </div>
      <div class="right-column">
        <p>
          We now choose a number <span class="math">k</span> of singular values that we are going to use for the approximation.
          The higher this number, the better the quality of the approximation gets but also the more data is needed to encode it.
          We now take only the first <span class="math">k</span> columns of <span class="math">U</span> and <span class="math">V</span> and the upper left <span class="math">(k × k)</span>-square of <span class="math">Σ</span>, containing the <span class="math">k</span> largest (and therefore most important) singular values.
          We then have
        </p>
        <div class="schema schema-b">
          <div class="matrix matrix-a">
            <div class="rows">m</div>
            <div class="cols">n</div>
            A
          </div>
          <div class="equals">≈</div>
          <div class="matrix matrix-u">
            <div class="range"></div>
            <div class="rows">m</div>
            <div class="cols">m</div>
            <div class="cols-k">k</div>
            U
          </div>
          <div class="mult-dot mult-dot-1"></div>
          <div class="matrix matrix-sigma">
            <div class="range"></div>
            <div class="rows">m</div>
            <div class="cols">n</div>
            <div class="cols-k">k</div>
            <div class="rows-k">k</div>
            <div class="sv" style="left: 0px; top: 0px;"></div>
            <div class="sv" style="left: 5px; top: 5px;"></div>
            <div class="sv unimportant" style="left: 10px; top: 10px;"></div>
            <div class="sv unimportant" style="left: 15px; top: 15px;"></div>
            <div class="sv unimportant" style="left: 20px; top: 20px;"></div>
            <div class="sv unimportant" style="left: 25px; top: 25px;"></div>
            <div class="sv unimportant" style="left: 30px; top: 30px;"></div>
            <div class="sv unimportant" style="left: 35px; top: 35px;"></div>
            <div class="sv unimportant" style="left: 40px; top: 40px;"></div>
            <div class="sv unimportant" style="left: 45px; top: 45px;"></div>
            Σ&nbsp;&nbsp;
          </div>
          <div class="mult-dot mult-dot-2"></div>
          <div class="matrix matrix-v">
            <div class="range"></div>
            <div class="rows">n</div>
            <div class="cols">n</div>
            <div class="rows-k">k</div>
            V <sup style="font-size: 0.7em;">T</sup>
          </div>
        </div>
        <p>
          The amount of data needed to store this approximation is proportional to the colored area:
        </p>
        <p class="center math">
          compressed size = <span class="u-color">m × k</span> + <span class="sigma-color">k</span> + <span class="v-color">k × n</span> = k × (<span class="sigma-color">1</span> + <span class="u-color">m</span> + <span class="v-color">n</span>)
        </p>
        <p>
          (Actually, slightly less space is needed due to the orthogonality of <span class="math">U</span> and <span class="math">V</span>.)
          One can prove that this approximation is <a href="https://en.wikipedia.org/wiki/Low-rank_approximation#Basic_low-rank_approximation_problem" title="Eckart–Young–Mirsky theorem">optimal in a certain sense</a>.
        </p>
        <p>
          This demo lets you choose the number of singular values <span class="math">k</span> and see how this choice affects the quality of the approximation and the compression rate.
          Notice how for all photographs, the graph showing the singular values looks like a hyperbola: there are only a few really large SVs and a long tail of relatively smaller SVs.
          In contrast, for the random noise image the graph of SVs looks roughly linear.
        </p>
        <p>
          SVD is routinely used in statistics for <a href="https://en.wikipedia.org/wiki/Principal_component_analysis">principal component analysis</a> and in numerical simulations for <a href="https://en.wikipedia.org/wiki/Model_order_reduction">reducing the order of models</a>.
          For image compression, more sophisticated methods like <a href="https://www.youtube.com/watch?v=n_uNPbdenRs">JPG</a> that take human perception into account generally outperform compression using SVD.
        </p>
        <h2>About this demo</h2>
        <p>
          The computation of the SVD is performed on the client-side using <a href="https://webassembly.org/">WebAssembly</a>.
          We use the algorithm implemented by the Rust library <a href="https://nalgebra.org/">nalgebra</a>.
          The SVDs of all three color channels are computed in parallel using one <a href="https://en.wikipedia.org/wiki/Web_worker">web worker</a> for every channel.
          To provide the quick preview, we use <a href="https://research.facebook.com/blog/294071574113354/fast-randomized-svd/">a randomized algorithm</a> to compute an approximate truncated SVD with 50 singular values.
          The user interface uses <a href="http://facebook.github.io/react/">React</a>, <a href="https://github.com/akiran/react-slick">react-slick</a> and <a href="http://refreshless.com/nouislider/">noUiSlider</a>.
          Thanks to the creators of all these great projects!
        </p>
      </div>
    </div>
    <div class="credits">
      <p>
        Built by <a href="http://github.com/timjb">Tim Baumann</a>. Fork this project on <a href="https://github.com/timjb/svd-image-compression-demo">GitHub</a>.
      </p>
    </div>
  </div>

  <script src="./SVD-Demo_ Image Compression_files/main.js.letöltés"></script>



</body></html>
