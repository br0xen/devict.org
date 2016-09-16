+++
title = "Binary Reader"
script = "/js/binary.js"
+++

<div class="container">
  <div class="row">
    <div class="col-xs-12 columns">
      <h1>Welcome SWE Expo!</h1>
      <p class="lead">Computers don't think and talk like us. Instead of English they speak Binary. <strong>Try writing a word in binary!</strong></p>

      <h3>What is Binary?</h3>
      <p>Binary numbers are just like regular numbers, except instead of using digits 0 through 9, they only use 0 and 1.</p>
    </div>
  </div>

  <div class="row">
    <div class="col-xs-7 columns">
      <h3>How to use</h3>
      <p>Each letter of the alphabet has a number. A is 1, B is 2, and so on. Figure out what number goes with each letter, and then click the holes to add the numbers up to equal that letters number.</p>
    </div>
    <div class="col-xs-5 columns">
      <p><strong>Brought to you by..</strong></p>
      <a href="http://makeict.org" title="MakeICT"><img src="/images/makeict-logo.png"></a>
    </div>
  </div>

  <button class="btn" id="clear">Clear</button>

  <table border="0" id="binary-reader-table">
    <thead>
      <tr id="word-input">
        <th colspan="2">Your Word:</th>
        <th>
          <input type="text" name="letter-0" value="">
        </th>
        <th>
          <input type="text" name="letter-1" value="">
        </th>
        <th>
          <input type="text" name="letter-2" value="">
        </th>
        <th>
          <input type="text" name="letter-3" value="">
        </th>
        <th>
          <input type="text" name="letter-4" value="">
        </th>
        <th>
          <input type="text" name="letter-5" value="">
        </th>
        <th>
          <input type="text" name="letter-6" value="">
        </th>
        <th>
          <input type="text" name="letter-7" value="">
        </th>
      </tr>
      <tr id="letter-position">
        <th colspan="2">Letter Position:</th>
        <th>
          <span id="letter-position-0"></span>
        </th>
        <th>
          <span id="letter-position-1"></span>
        </th>
        <th>
          <span id="letter-position-2"></span>
        </th>
        <th>
          <span id="letter-position-3"></span>
        </th>
        <th>
          <span id="letter-position-4"></span>
        </th>
        <th>
          <span id="letter-position-5"></span>
        </th>
        <th>
          <span id="letter-position-6"></span>
        </th>
        <th>
          <span id="letter-position-7"></span>
        </th>
    </thead>
    <tbody>
      <tr>
        <td></td>
        <td>16</td>
        <td data-letter="0" data-hole="0" data-value="16" class="hole"><span></span></td>
        <td data-letter="1" data-hole="0" data-value="16" class="hole"><span></span></td>
        <td data-letter="2" data-hole="0" data-value="16" class="hole"><span></span></td>
        <td data-letter="3" data-hole="0" data-value="16" class="hole"><span></span></td>
        <td data-letter="4" data-hole="0" data-value="16" class="hole"><span></span></td>
        <td data-letter="5" data-hole="0" data-value="16" class="hole"><span></span></td>
        <td data-letter="6" data-hole="0" data-value="16" class="hole"><span></span></td>
        <td data-letter="7" data-hole="0" data-value="16" class="hole"><span></span></td>
      </tr>
      <tr>
        <td></td>
        <td>8</td>
        <td data-letter="0" data-hole="1" data-value="8" class="hole"><span></span></td>
        <td data-letter="1" data-hole="1" data-value="8" class="hole"><span></span></td>
        <td data-letter="2" data-hole="1" data-value="8" class="hole"><span></span></td>
        <td data-letter="3" data-hole="1" data-value="8" class="hole"><span></span></td>
        <td data-letter="4" data-hole="1" data-value="8" class="hole"><span></span></td>
        <td data-letter="5" data-hole="1" data-value="8" class="hole"><span></span></td>
        <td data-letter="6" data-hole="1" data-value="8" class="hole"><span></span></td>
        <td data-letter="7" data-hole="1" data-value="8" class="hole"><span></span></td>
      </tr>
      <tr>
        <td></td>
        <td>4</td>
        <td data-letter="0" data-hole="2" data-value="4" class="hole"><span></span></td>
        <td data-letter="1" data-hole="2" data-value="4" class="hole"><span></span></td>
        <td data-letter="2" data-hole="2" data-value="4" class="hole"><span></span></td>
        <td data-letter="3" data-hole="2" data-value="4" class="hole"><span></span></td>
        <td data-letter="4" data-hole="2" data-value="4" class="hole"><span></span></td>
        <td data-letter="5" data-hole="2" data-value="4" class="hole"><span></span></td>
        <td data-letter="6" data-hole="2" data-value="4" class="hole"><span></span></td>
        <td data-letter="7" data-hole="2" data-value="4" class="hole"><span></span></td>
      </tr>
      <tr>
        <td></td>
        <td>2</td>
        <td data-letter="0" data-hole="3" data-value="2" class="hole"><span></span></td>
        <td data-letter="1" data-hole="3" data-value="2" class="hole"><span></span></td>
        <td data-letter="2" data-hole="3" data-value="2" class="hole"><span></span></td>
        <td data-letter="3" data-hole="3" data-value="2" class="hole"><span></span></td>
        <td data-letter="4" data-hole="3" data-value="2" class="hole"><span></span></td>
        <td data-letter="5" data-hole="3" data-value="2" class="hole"><span></span></td>
        <td data-letter="6" data-hole="3" data-value="2" class="hole"><span></span></td>
        <td data-letter="7" data-hole="3" data-value="2" class="hole"><span></span></td>
      </tr>
      <tr>
        <td></td>
        <td>1</td>
        <td data-letter="0" data-hole="4" data-value="1" class="hole"><span></span></td>
        <td data-letter="1" data-hole="4" data-value="1" class="hole"><span></span></td>
        <td data-letter="2" data-hole="4" data-value="1" class="hole"><span></span></td>
        <td data-letter="3" data-hole="4" data-value="1" class="hole"><span></span></td>
        <td data-letter="4" data-hole="4" data-value="1" class="hole"><span></span></td>
        <td data-letter="5" data-hole="4" data-value="1" class="hole"><span></span></td>
        <td data-letter="6" data-hole="4" data-value="1" class="hole"><span></span></td>
        <td data-letter="7" data-hole="4" data-value="1" class="hole"><span></span></td>
      </tr>
    </tbody>
  </table>
</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery.touchswipe/1.6.4/jquery.touchSwipe.min.js"></script>
