## why

Because when I sorted files by "Date Modified", I expect next/previous navigation in my image viewer to mirror what I would have within the file manager

## how

A Python wrapper script for `imv` that queries Thunar's folder sorting metadata (`metadata::thunar-sort-column` and `metadata::thunar-sort-order`) using `gio info`. It filters the directory's files for images, sorts them exactly like Thunar does (respecting Thunar's smart-sort configuration), and launches `imv` with the sorted list starting at the selected image.

## Usage

1. Install:
```
git clone https://github.com/Taugeshtu/imv-dir-respect
mkdir -p ~/.local/bin
cp imv-dir-respect/imv-dir-respect ~/.local/bin
cp imv-dir-respect/imv-dir.desktop ~/.local/share/applications
chmod +x ~/.local/bin/imv-dir-respect
update-desktop-database ~/.local/share/applications
rm -r imv-dir-respect
```
2. Set `imv-dir` as your image opener
3. ...
4. PROFIT!

