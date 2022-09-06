# cs-con-binary-struct-writer

- ### [Microsoft : 構造体のマーシャリングをカスタマイズする](https://docs.microsoft.com/ja-jp/dotnet/standard/native-interop/customize-struct-marshalling)

```cs
struct BinaryData {
    public float item1;
    [MarshalAs(UnmanagedType.ByValTStr, SizeConst = 8)]
    public string item2;
    public Int32 item3;
    public bool item4;

    public BinaryData(float a, string b, Int32 c, bool d)
    {
        this.item1 = a;
        this.item2 = b;
        this.item3 = c;
        this.item4 = d;

    }
}
```
