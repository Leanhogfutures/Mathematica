# Mathematica

<math xmlns='http://www.w3.org/1998/Math/MathML'
    mathematica:form='StandardForm'
    xmlns:mathematica='http://www.wolfram.com/XML/'>
 <mrow>
  <mrow>
   <mi>F</mi>
   <mo>[</mo>
   <mi>n_</mi>
   <mo>]</mo>
  </mrow>
  <mo>:=</mo>
  <mrow>
   <mfrac>
    <mrow>
     <mi>a</mi>
     <mo>[</mo>
     <mn>0</mn>
     <mo>]</mo>
    </mrow>
    <mn>2</mn>
   </mfrac>
   <mo>+</mo>
   <mrow>
    <munderover>
     <mo>&#8721;</mo>
     <mrow>
      <mi>r</mi>
      <mo>=</mo>
      <mn>1</mn>
     </mrow>
     <mi>n</mi>
    </munderover>
    <mrow>
     <mo>(</mo>
     <mrow>
      <mrow>
       <mi>ar</mi>
       <mo>&#8290;</mo>
       <mrow>
        <mi>Cos</mi>
        <mo>[</mo>
        <mfrac>
         <mrow>
          <mn>2</mn>
          <mo>&#8290;</mo>
          <mi>&#960;</mi>
          <mo>&#8290;</mo>
          <mi>r</mi>
          <mo>&#8290;</mo>
          <mi>x</mi>
         </mrow>
         <mi>L</mi>
        </mfrac>
        <mo>]</mo>
       </mrow>
      </mrow>
      <mo>+</mo>
      <mtext> </mtext>
      <mrow>
       <mi>br</mi>
       <mo>&#8290;</mo>
       <mrow>
        <mi>Sin</mi>
        <mo>[</mo>
        <mfrac>
         <mrow>
          <mn>2</mn>
          <mo>&#8290;</mo>
          <mi>&#960;</mi>
          <mo>&#8290;</mo>
          <mi>r</mi>
          <mo>&#8290;</mo>
          <mi>x</mi>
         </mrow>
         <mi>L</mi>
        </mfrac>
        <mo>]</mo>
       </mrow>
      </mrow>
     </mrow>
     <mo>)</mo>
    </mrow>
   </mrow>
  </mrow>
 </mrow>
</math>

<math xmlns='http://www.w3.org/1998/Math/MathML'
    mathematica:form='StandardForm'
    xmlns:mathematica='http://www.wolfram.com/XML/'>
 <mrow>
  <mrow>
   <mi>G1</mi>
   <mo>=</mo>
   <mrow>
    <mrow>
     <mi>FourierTransform</mi>
     <mo>[</mo>
     <mrow>
      <mrow>
       <mi>g</mi>
       <mo>[</mo>
       <mi>t</mi>
       <mo>]</mo>
      </mrow>
      <mo>,</mo>
      <mi>x</mi>
      <mo>,</mo>
      <mi>k</mi>
      <mo>,</mo>
      <mrow>
       <mi>FourierParameters</mi>
       <semantics>
        <mo>&#8594;</mo>
        <annotation encoding='Mathematica'>&quot;->&quot;</annotation>
       </semantics>
       <mrow>
        <mo>{</mo>
        <mrow>
         <mn>0</mn>
         <mo>,</mo>
         <mrow>
          <mo>-</mo>
          <mn>1</mn>
         </mrow>
        </mrow>
        <mo>}</mo>
       </mrow>
      </mrow>
     </mrow>
     <mo>]</mo>
    </mrow>
    <mo>//</mo>
    <mrow>
     <mrow>
      <mi>Simplify</mi>
      <mo>[</mo>
      <mrow>
       <mi>#</mi>
       <mo>,</mo>
       <mrow>
        <mi>t</mi>
        <mo>&gt;</mo>
        <mn>0</mn>
       </mrow>
      </mrow>
      <mo>]</mo>
     </mrow>
     <mo>&amp;</mo>
    </mrow>
   </mrow>
  </mrow>
  <mo>&#8290;</mo>
  <mtext>&#62371;</mtext>
  <mtext> </mtext>
  <mrow>
   <mi>Plot</mi>
   <mo>[</mo>
   <mrow>
    <mrow>
     <mi>Evaluate</mi>
     <mo>[</mo>
     <mrow>
      <mi>Table</mi>
      <mo>[</mo>
      <mrow>
       <mrow>
        <mi>g</mi>
        <mo>[</mo>
        <mi>t</mi>
        <mo>]</mo>
       </mrow>
       <mo>,</mo>
       <mrow>
        <mo>{</mo>
        <mrow>
         <mi>t</mi>
         <mo>,</mo>
         <mn>0.1</mn>
         <mo>,</mo>
         <mn>1.</mn>
         <mo>,</mo>
         <mn>0.1</mn>
        </mrow>
        <mo>}</mo>
       </mrow>
      </mrow>
      <mo>]</mo>
     </mrow>
     <mo>]</mo>
    </mrow>
    <mo>,</mo>
    <mrow>
     <mo>{</mo>
     <mrow>
      <mi>k</mi>
      <mo>,</mo>
      <mrow>
       <mo>-</mo>
       <mn>5</mn>
      </mrow>
      <mo>,</mo>
      <mn>5</mn>
     </mrow>
     <mo>}</mo>
    </mrow>
    <mo>,</mo>
    <mtext> </mtext>
    <mrow>
     <mi>PlotStyle</mi>
     <semantics>
      <mo>&#8594;</mo>
      <annotation encoding='Mathematica'>&quot;->&quot;</annotation>
     </semantics>
     <mrow>
      <mi>Table</mi>
      <mo>[</mo>
      <mrow>
       <mrow>
        <mo>{</mo>
        <mrow>
         <mrow>
          <mi>Hue</mi>
          <mo>[</mo>
          <mrow>
           <mn>0.1</mn>
           <mtext> </mtext>
           <mi>i</mi>
          </mrow>
          <mo>]</mo>
         </mrow>
         <mo>,</mo>
         <mi>Thick</mi>
        </mrow>
        <mo>}</mo>
       </mrow>
       <mo>,</mo>
       <mrow>
        <mo>{</mo>
        <mrow>
         <mi>i</mi>
         <mo>,</mo>
         <mn>0</mn>
         <mo>,</mo>
         <mn>10</mn>
        </mrow>
        <mo>}</mo>
       </mrow>
      </mrow>
      <mo>]</mo>
     </mrow>
    </mrow>
    <mo>,</mo>
    <mrow>
     <mi>PlotRange</mi>
     <semantics>
      <mo>&#8594;</mo>
      <annotation encoding='Mathematica'>&quot;->&quot;</annotation>
     </semantics>
     <mrow>
      <mo>{</mo>
      <mrow>
       <mrow>
        <mo>{</mo>
        <mrow>
         <mrow>
          <mo>-</mo>
          <mn>5</mn>
         </mrow>
         <mo>,</mo>
         <mn>5</mn>
        </mrow>
        <mo>}</mo>
       </mrow>
       <mo>,</mo>
       <mrow>
        <mo>{</mo>
        <mrow>
         <mn>0</mn>
         <mo>,</mo>
         <mn>0.5</mn>
        </mrow>
        <mo>}</mo>
       </mrow>
      </mrow>
      <mo>}</mo>
     </mrow>
    </mrow>
    <mo>,</mo>
    <mtext>&#62371;</mtext>
    <mrow>
     <mi>AxesLabel</mi>
     <semantics>
      <mo>&#8594;</mo>
      <annotation encoding='Mathematica'>&quot;->&quot;</annotation>
     </semantics>
     <mrow>
      <mo>{</mo>
      <mrow>
       <ms>k</ms>
       <mo>,</mo>
       <ms>F1</ms>
      </mrow>
      <mo>}</mo>
     </mrow>
    </mrow>
    <mo>,</mo>
    <mtext> </mtext>
    <mrow>
     <mi>Background</mi>
     <semantics>
      <mo>&#8594;</mo>
      <annotation encoding='Mathematica'>&quot;->&quot;</annotation>
     </semantics>
     <mi>LightGray</mi>
    </mrow>
   </mrow>
   <mo>]</mo>
  </mrow>
 </mrow>
</math>