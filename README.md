# IDM + 18.2 edited
this is an altered version of IDM+ for android 

added large mapping file 

added data hosts for opening links

completed implementing termux into the app

completed implementing shizuku into the app

This is a work in progress any insight is appreciated as i am just learning 

make sure to use the run command for the termux app

value="true"; key="allow-external-apps"; file="/data/data/com.termux/files/home/.termux/termux.properties"; mkdir -p "$(dirname "$file")"; chmod 700 "$(dirname "$file")"; if ! grep -E '^'"$key"'=.*' $file &>/dev/null; then [[ -s "$file" && ! -z "$(tail -c 1 "$file")" ]] && newline=$'\n' || newline=""; echo "$newline$key=$value" >> "$file"; else sed -i'' -E 's/^'"$key"'=.*/'"$key=$value"'/' $file; fi

GOOGLE TRANSLATE CURRENT PAGE!!

Added google translate button to browser to show on all webpages visited

BUG!! "Some websites may need to be first loaded as desktop view to see all available language selections the first time and shpuld renember language selection per page with cookies enabled" (will remedy the view issue in a later release)

Some websites may not allow this button to work based on CORS or other blockers

Whats Next

began implemening an internal CLI 

began vpn integration


