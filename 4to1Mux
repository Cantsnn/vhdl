-------------------------------------------
-- İsmailcan Tosun 365239 Say.Tas.Lab. Deneyi
-- 1 bit girisli 4-1 Multiplexer
-- Girisler : a,b,c,d,s0,s1
-- Cikis : f
-------------------------------------------

Library IEEE;
Use ieee.std_logic_1164.all; -- Standart tanimlamalar

Entity eMux is --port tanımlamalari
port(   a,b,c,d : in std_logic; --1 bit girisli oldugu icin bu yapiyi kullaniyoruz.
	   s0,s1: in std_logic;  -- daha fazla bit girisi icin vector yapisi kullanilir.
               f : out std_logic);
End eMux;


Architecture Behv of eMux is    --yapisini tanımlama
Begin
	        f <=  a When s0='0' and s1='0' Else   --ilgili giris gelirse o girisi cikisa verecek if yapısı da kullanılabilir.
		      b When s0='0' and s1='1' Else
		      c When s0='1' and s1='0' Else
		      d When s0='1' and s1='1' Else
		      '0'; --farklı bir giris gelirse sifir gosterecek.
End Behv;
