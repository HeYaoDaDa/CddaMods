# HeYaoDaDa Cdda Mod

Cataclysm-DDA's mod

## Note

json format: https://dev.narc.ro/cataclysm/format.html

gettext commod:
```bash
mkdir -p ./mod/lang/po
python3 CDDA-repo/lang/extract_json_strings.py -i ./mod -o ./mod/lang/po/mod.pot
msginit -o ./mod/lang/po/zh_CN.po -i ./mod/lang/po/mod.pot -l zh_CN
mkdir -p mod/lang/mo/zh_CN/LC_MESSAGES/
msgfmt -o mod/lang/mo/zh_CN/LC_MESSAGES/mod.mo mod/lang/po/zh_CN.po
```

release zip commod: `zip -r mod.zip mod -x mod/lang/po\*`