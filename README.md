# node_sbom

```
// コードと同じ階層にあるファイルとフォルダを取得
dir, err := os.Getwd()
if err != nil {
  panic(err)
}
files, _ := ioutil.ReadDir(filepath.Join(dir, "build"))
if len(files) != 1 {
  log.Fatalln("There are multiple files in the build directory. Delete the files in the directory and retry.")
}
out, err := exec.Command().Output()
if err != nil {
  log.Fatal(err)
}
fmt.Println(string(out))


```
