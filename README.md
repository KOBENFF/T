--[[
This script is protected by XProtect Obfuscator Free Version.

Version: 1.0
Obfuscation Time: 709ms

For support and updates, join our Discord community:
Discord: discord.gg/7hv7k6FfNr

]]
local t=string.byte;local r=string.char;local c=string.sub;local s=table.concat;local b=math.ldexp;local S=getfenv or function()return _ENV end;local l=setmetatable;local f=select;local i=unpack;local h=tonumber;local function u(t)local e,o,a="","",{}local n=256;local d={}for l=0,n-1 do d[l]=r(l)end;local l=1;local function f()local e=h(c(t,l,l),36)l=l+1;local o=h(c(t,l,l+e-1),36)l=l+e;return o end;e=r(f())a[1]=e;while l<#t do local l=f()if d[l]then o=d[l]else o=e..c(e,1,1)end;d[n]=e..c(o,1,1)a[#a+1],e,n=o,o,n+1 end;return table.concat(a)end;local a=u('25827425825427525825227525S25V26526025R25K25Q25X25U26327627526326525T26125825727526S25K25K25O26Z26125K25827227525W27W25O25R23Q24324325Q26525N24226325X25K25W25L26625L25R26125Q26725V25U25K26128S24228Q25T24326V26R27226X26Q26Y26Y26Z26Z26S26S28Z26R23T23U23V24325T26527J24326M26X27126W26P26X24225T26025825127524C25022421V25725027424824S29Z25324S27424925023W2582532A225824024C2A624C27423X2AF2AE2A92AK2AD2AQ24D2582AK25327524D2502A82AO2582AY2742B1');local n=bit and bit.bxor or function(l,e)local o,n=1,0 while l>0 and e>0 do local c,a=l%2,e%2 if c~=a then n=n+o end l,e,o=(l-c)/2,(e-a)/2,o*2 end if l<e then l=e end while l>0 do local e=l%2 if e>0 then n=n+o end l,o=(l-e)/2,o*2 end return n end local function l(e,l,o)if o then local l=(e/2^(l-1))%2^((o-1)-(l-1)+1);return l-l%1;else local l=2^(l-1);return(e%(l+l)>=l)and 1 or 0;end;end;local e=1;local function o()local a,c,l,o=t(a,e,e+3);a=n(a,188)c=n(c,188)l=n(l,188)o=n(o,188)e=e+4;return(o*16777216)+(l*65536)+(c*256)+a;end;local function d()local l=n(t(a,e,e),188);e=e+1;return l;end;local function Q()local e=o();local n=o();local c=1;local o=(l(n,1,20)*(2^32))+e;local e=l(n,21,31);local l=((-1)^l(n,32));if(e==0)then if(o==0)then return l*0;else e=1;c=0;end;elseif(e==2047)then return(o==0)and(l*(1/0))or(l*(0/0));end;return b(l,e-1023)*(c+(o/(2^52)));end;local h=o;local function b(l)local o;if(not l)then l=h();if(l==0)then return'';end;end;o=c(a,e,e+l-1);e=e+l;local e={}for l=1,#o do e[l]=r(n(t(c(o,l,l)),188))end return s(e);end;local e=o;local function u(...)return{...},f('#',...)end local function K()local t={0,0,0,0,0,0,0,0,0};local e={};local c={};local a={t,nil,e,nil,c};for l=1,o()do e[l-1]=K();end;local e=o()local c={0,0,0,0};for o=1,e do local e=d();local l;if(e==1)then l=(d()~=0);elseif(e==2)then l=Q();elseif(e==0)then l=b();end;c[o]=l;end;a[2]=c a[4]=d();for a=1,o()do local c=n(o(),33);local o=n(o(),11);local n=l(c,1,2);local e=l(o,1,11);local e={e,l(c,3,11),nil,nil,o};if(n==0)then e[3]=l(c,12,20);e[5]=l(c,21,29);elseif(n==1)then e[3]=l(o,12,33);elseif(n==2)then e[3]=l(o,12,32)-1048575;elseif(n==3)then e[3]=l(o,12,32)-1048575;e[5]=l(c,21,29);end;t[a]=e;end;return a;end;local function Q(l,e,h)local e=l[1];local n=l[2];local o=l[3];local l=l[4];return function(...)local r=e;local t=n;local e=o;local n=l;local b=u local o=1;local d=-1;local u={};local a={...};local c=f('#',...)-1;local l={};local e={};for l=0,c do if(l>=n)then u[l-n]=a[l+1];else e[l]=a[l+1];end;end;local l=c-n+1 local l;local n;while true do l=r[o];n=l[1];if n<=7 then if n<=3 then if n<=1 then if n==0 then e[l[2]]=h[t[l[3]]];else local o=l[2];local n=e[l[3]];e[o+1]=n;e[o]=n[t[l[5]]];end;elseif n>2 then e[l[2]]=(l[3]~=0);else local n=l[2];local c={};local o=0;local l=n+l[3]-1;for l=n+1,l do o=o+1;c[o]=e[l];end;local c,l=b(e[n](i(c,1,l-n)));l=l+n-1;o=0;for l=n,l do o=o+1;e[l]=c[o];end;d=l;end;elseif n<=5 then if n>4 then e[l[2]]();d=A;else e[l[2]]();d=A;end;elseif n>6 then do return end;else e[l[2]]=h[t[l[3]]];end;elseif n<=11 then if n<=9 then if n>8 then e[l[2]]=(l[3]~=0);else e[l[2]]=t[l[3]];end;elseif n>10 then local o=l[2];local n=e[l[3]];e[o+1]=n;e[o]=n[t[l[5]]];else do return end;end;elseif n<=13 then if n>12 then local n=l[2];local c={};local o=0;local a=d;for l=n+1,a do o=o+1;c[o]=e[l];end;local c={e[n](i(c,1,a-n))};local l=n+l[5]-2;o=0;for l=n,l do o=o+1;e[l]=c[o];end;d=l;else local n;local u,n;local a;local c;local f;local s;local n;e[l[2]]=h[t[l[3]]];o=o+1;l=r[o];e[l[2]]=h[t[l[3]]];o=o+1;l=r[o];n=l[2];s=e[l[3]];e[n+1]=s;e[n]=s[t[l[5]]];o=o+1;l=r[o];e[l[2]]=t[l[3]];o=o+1;l=r[o];e[l[2]]=(l[3]~=0);o=o+1;l=r[o];n=l[2];f={};c=0;a=n+l[3]-1;for l=n+1,a do c=c+1;f[c]=e[l];end;u,a=b(e[n](i(f,1,a-n)));a=a+n-1;c=0;for l=n,a do c=c+1;e[l]=u[c];end;d=a;o=o+1;l=r[o];n=l[2];f={};c=0;a=d;for l=n+1,a do c=c+1;f[c]=e[l];end;u={e[n](i(f,1,a-n))};a=n+l[5]-2;c=0;for l=n,a do c=c+1;e[l]=u[c];end;d=a;o=o+1;l=r[o];e[l[2]]();d=n;o=o+1;l=r[o];do return end;end;elseif n<=14 then local n=l[2];local c={};local o=0;local l=n+l[3]-1;for l=n+1,l do o=o+1;c[o]=e[l];end;local c,l=b(e[n](i(c,1,l-n)));l=l+n-1;o=0;for l=n,l do o=o+1;e[l]=c[o];end;d=l;elseif n==15 then e[l[2]]=t[l[3]];else local n=l[2];local a={};local o=0;local c=d;for l=n+1,c do o=o+1;a[o]=e[l];end;local c={e[n](i(a,1,c-n))};local l=n+l[5]-2;o=0;for l=n,l do o=o+1;e[l]=c[o];end;d=l;end;o=o+1;end;end;end;return Q(K(),{},S())();
