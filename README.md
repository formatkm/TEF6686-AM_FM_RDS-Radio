HIgh performance AM/FM RDS software-defined radio signal processing tuner with TEF6686 and I2C Arduino Controller for XDR/NXP/TEF GTK user interface
 ( for old "historical" versions visit rdi.boards.net ! )
      
On genuine XDR-GTK interface the de-emphasis switch is acting now this way:

  50uS => NORMAL ( 50 uS );
  
  75uS => FLAT ( 0 uS );
  
  0uS  => MPX out mode ( DAC_Left : FM MPX (DARC) signal / DAC_Right : mono audio );
  
XDR-GTK Antenna Switch option:

  Ant A = Normal
  
  Ant B = iMS enabled ( FM multipath suppression when the receiver is in a moving vehicle )
  
  Ant C = EQ enabled ( FM channel equalizer for improved field performance )
  
  Ant D = Both enabled
  
Audio output level is fixed -> 0dB or +3dB
  
For AM the following four bandwidth settings are supported:

    3 / 4 / 6 / 8 kHz

For FM the following sixteen bandwidth settings are supported:

    56 / 64 / 72 / 84 / 97 / 114 / 133 / 151 / 168 / 184 / 200 / 217 / 236 / 254 / 287 / 311 kHz

Other bandwidth parameter values are rounded to the nearest supported bandwidth in genuine XDR-GTK user interface but
in the NXP/TEF-GTK modified user interfaces the bandwidth parameter values fits well.

In some third party XDR-GTK altered versions available on internet the word "Ant" has been replaced by others such as the funny "DX", which, apart from the word itself on a button, doesn't bring a real "DX" plus of performance on weak fringe RF signals, being only just linked to some variations of tone corrections through DSP that modify the audio signal after demodulation to impress the fools :)
  
Great special thanks to Konrad Kosmatka, author of the original & brilliant version for Sony XDR-F1HD
 
 https://fmdx.pl/xdr-i2c/
 
 https://fmdx.pl/xdr-gtk/
  
  and also to ( in alphabetical order ):

  - ace919
  - Brian Beezley
  - dxhdtv
  - eggplant886
  - fmdxbp
  - Jan Kolar
  - Marcin Woloszczuk
  - Mihai Popa          https://github.com/stailus/tef6686_rds
  - makserge            https://github.com/makserge/tef6686_radio
  - Nicu Florica        http://nicuflorica.blogspot.com/2020/02/radio-cu-tef6686.html
  - ODJeetje
  - Olivier Guillaume
  - Przemyslaw Korpas
  - Sjef Verhoeven      https://github.com/PE5PVB
  - VoXiTPro            https://github.com/voxit1512/Tef6686

  and many other enthusiasts ...

  Tested on Arduino Nano V3.0 at 5V

  Feel free to add your own contribution to this nice project !
