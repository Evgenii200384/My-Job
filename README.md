
Delphi:

program for_tshirt;
var
  s, k : string;
  i, php, javascript : integer;
begin
  readln(s);
  k := '';
  for i := 1 to length(s) do
    if (s[i] = ' ') or (s[i] in ['a'..'z']) or (s[i] in ['A'..'Z']) then 
      k := k + upcase(s[i]);
  php := 0;
  javascript := 0;
  k := ' ' + k + ' ';
  for i := 1 to length(k) do begin
    if (length(k) - i >= 4) then 
      inc(php, ord(copy(k, i, 5) = ' PHP ')));
    if (length(k) - i >= 9) then 
      inc(javascript, ord(copy(k, i, 10) = ' JAVASCRIPT ')));
  end;
  if (php > javascript) then 
    writeln('PHP')
  else
    if (php < javascript) then 
      writeln('JavaScript')
    else
      writeln('C++ or Java or Python');
end.# My-Job
