# TUGAS WEBSERVICE

**Oleh :**

**Nama        : Muthmainnah**

**NPM        : 1144050**

**Kelas        : D4 TI 3B**





**PROGRAM DIPLOMA IV TEKNIK INFORMATIKA**

**POLITEKNIK POS INDONESIA**

**BANDUNG**

**2017**

&lt;?xmlversion=_&quot;1.0&quot;_encoding=_&quot;UTF-8&quot;_?&gt;&lt;!DOCTYPElogbarangSYSTEM&quot;logbarang.dtd&quot;&gt;

&lt;logbarang&gt;

&lt;barang&gt;

    &lt;kode&gt;M1112&lt;/kode&gt;

    &lt;satuan&gt;pc&lt;/satuan&gt;

    &lt;hargacur=_&quot;nmtoken&quot;_&gt;5000&lt;/harga&gt;

    &lt;asal&gt;

            &lt;pt&gt;ladyrock&lt;/pt&gt;

        &lt;kodewil&gt;10&lt;/kodewil&gt;

    &lt;/asal&gt;

    &lt;tujuan&gt;

            &lt;pt&gt;union&lt;/pt&gt;

        &lt;kodewil&gt; 1001 &lt;/kodewil&gt;

    &lt;/tujuan&gt;

&lt;/barang&gt;

    &lt;barang&gt;

                    &lt;kode&gt;M1122&lt;/kode&gt;

            &lt;satuan&gt;pc&lt;/satuan&gt;

            &lt;harga&gt;1000&lt;/harga&gt;

            &lt;asal&gt;

                    &lt;pt&gt;pmb&lt;/pt&gt;

                &lt;kodewil&gt;103&lt;/kodewil&gt;

                        &lt;/asal&gt;

            &lt;tujuan&gt;

                    &lt;pt&gt;mitrakencana&lt;/pt&gt;

                &lt;kodewil&gt;300&lt;/kodewil&gt;

             &lt;/tujuan&gt;

&lt;/barang&gt;

&lt;/logbarang&gt;

**ANALISIS**

Sintak untuk memulai pembuatan sintak xml

|  &lt;?xmlversion=_&quot;1.0&quot;_encoding=_&quot;UTF-8&quot;_?&gt;  |
| --- |

Sintak yang menyatakan bahwa dtd dengan logbarang sudah terhubung dengan xmlnya.

|  &lt;!DOCTYPElogbarangSYSTEM&quot;logbarang.dtd&quot;&gt;  |
| --- |

Sintak element logbarang dari xml dengan nama barang.

|  &lt;logbarang&gt;  |
| --- |

Dalam elemen logbarang terdapat elemen barang dengan didalamnya terdapat element kode, satuan, harga, asal, dan tujuan. Dalam elemen harga terdapat atribut cur = &quot;nmtoken&quot;. Dalam elemen asal terdapat elemen pt dan kodewil dan dalam elemen tujuan terdapat elemen pt dan kodewil. Dan ditutup dengan elemen penutul barang.

|  &lt;barang&gt;          &lt;kode&gt;M1112&lt;/kode&gt;          &lt;satuan&gt;pc&lt;/satuan&gt;          &lt;hargacur=_&quot;nmtoken&quot;_&gt;5000&lt;/harga&gt;          &lt;asal&gt;                  &lt;pt&gt;ladyrock&lt;/pt&gt;                     &lt;kodewil&gt;10&lt;/kodewil&gt;          &lt;/asal&gt;        &lt;tujuan&gt;                             &lt;pt&gt;union&lt;/pt&gt;                             &lt;kodewil&gt;1001&lt;/kodewil&gt;          &lt;/tujuan&gt;&lt;/barang&gt;    |
| --- |

Penutup elemen logbarang.

Logbarang.dtd

|  &lt;/logbarang&gt;  |
| --- |



Sintak yang digunakan pada awal dtd.

|  &lt;?xml encoding=&quot;UTF-8&quot;?&gt;  |
| --- |

Dalam element dtd logbarang terdapat element dengan nama &quot;barang&quot;. Terdapat tanda &quot;+&quot; ini menyatakan bahwa data pada element barang harus ada minimal 1 atau lebih.

|  &lt;!ELEMENTlogbarang (barang)+&gt;  |
| --- |

Attlist menyatakan nama element dalam xml.

|  &lt;!ATTLISTlogbarang    xmlns CDATA#FIXED_&#39;&#39;_&gt;  |
| --- |

Pada elemen barang didalamnya terdapat element lain yaitu kode, satuan, harga, asal dan tujuan. Tanda &quot;?&quot; menyatakan bahwa elemen yang memiliki tanda tersebut boleh tidak memiliki data atau bisa memiliki data.

|  &lt;!ELEMENTbarang (kode?,satuan,harga,asal,tujuan)&gt;  |
| --- |

Pada elemen kode berisi data atau value. Dengan nama elemen di xml kode.

|  &lt;!ELEMENTkode(#PCDATA)&gt;&lt;!ATTLISTkode    xmlns CDATA#FIXED_&#39;&#39;_&gt;  |
| --- |

Pada elemen satuan berisi data atau value. Dengan nama elemen di xml satuan.

|  &lt;!ELEMENTsatuan(#PCDATA)&gt;&lt;!ATTLISTsatuan    xmlns CDATA#FIXED_&#39;&#39;_&gt;  |
| --- |

Pada elemen harga berisi data atau value. Dengan nama elemen di xml harga dan atribut cur dengan nilai nmtoken.

|  &lt;!ELEMENTharga(#PCDATA)&gt;&lt;!ATTLISTharga    xmlns CDATA#FIXED_&#39;&#39;_    cur NMTOKEN#IMPLIED&gt;  |
| --- |

Pada elemen asal didalamnya terdapat elemen pt dan kodewil.

|  &lt;!ELEMENTasal (pt,kodewil)&gt;&lt;!ATTLISTasal    xmlns CDATA#FIXED_&#39;&#39;_&gt;  |
| --- |

Pada elemen tujuan didalamnya terdapat elemen pt dan kodewil.

|  &lt;!ELEMENTtujuan (pt,kodewil)&gt;&lt;!ATTLISTtujuan    xmlns CDATA#FIXED_&#39;&#39;_&gt;  |
| --- |

Pada elemen pt berisi data atau value. Dengan nama elemen di xml pt.

|  &lt;!ELEMENTpt(#PCDATA)&gt;&lt;!ATTLISTpt    xmlns CDATA#FIXED_&#39;&#39;_&gt;  |
| --- |

Pada elemen kodewil berisi data atau value. Dengan nama elemen di xml kodewil.

|  &lt;!ELEMENTkodewil(#PCDATA)&gt;&lt;!ATTLISTkodewil    xmlns CDATA#FIXED_&#39;&#39;_&gt; |
| --- |