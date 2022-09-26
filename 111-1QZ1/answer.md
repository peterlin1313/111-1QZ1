# 第1次隨堂-隨堂-QZ1
>
>學號：109111110
><br />
>姓名：林育德
><br />
>作業撰寫時間：30 (mins，包含程式撰寫時間)
><br />
>最後撰寫文件日期：2022/9/26
>

本份文件包含以下主題：(至少需下面兩項，若是有多者可以自行新增)
- [x]說明內容
- [x]個人認為完成作業須具備觀念

## 說明程式與內容
生成一個整數2維陣列變數大小為10* 10
生成一個整數1維陣列變數大小為10，名稱為ia_MIndex。 在ia_Map，即10*10的二維陣列中，其索引值
從0至99。今有10個地雷儲存於ia_MIndex，其生成點於索引值0至99中
輸入 0 7 13 28 44 62 74 75 87 90 輸出為下面陣列

namespace _111_1QZ1
{
    public partial class Bomb : System.Web.UI.Page
    {
        protected void Page_Load(object sender, EventArgs e)
        {
            int[] ia_MIndex = new int[10] {0, 7, 13, 28, 44, 62, 74, 75, 87, 90 };
            char[,] ia_Map = new char[10, 10];
            for (int i_Row=0; i_Row< 10; i_Row++) {
                for (int i_Col = 0; i_Col < 10; i_Col++) {
                    ia_Map[i_Row, i_Col] = 'o';
                }
            }


            for (int i_Ct = 0; i_Ct <10; i_Ct++)
            {
                int i_Row = ia_MIndex[i_Ct] / 10;
                int i_Col = ia_MIndex[i_Ct] % 10;
                ia_Map[i_Row, i_Col] = '*';
            }


            for(int i_Row = 0; i_Row < 10; i_Row++)
            {
                for (int i_Col = 0; i_Col < 10; i_Col++)
                {
                        Response.Write(ia_Map[i_Row, i_Col]);
                }
                Response.Write("<br>");

## 個人認為完成作業須具備觀念

開始寫說明，需要說明本次作業個人覺得需學會那些觀念 (需寫成文章，需最少50字，
並且文內不得有你、我、他三種文字)

