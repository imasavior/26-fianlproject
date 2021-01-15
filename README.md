# 26組-finalproject
=======
成員:108321050，
對打遊戲

功能說明:
紅色與綠色玩家對戰，在時間結束後最高分者獲勝。
在8x8 LED 矩陣，用來顯示對戰畫面

7段顯示器顯示剩餘生命(從5開始)

當A攻擊B時，攻擊判定成功，5+=1。

當B攻擊A時，攻擊判定成功，5-=1。

當A攻擊B時，B使用格擋，攻擊判定失敗，不扣分。

當B攻擊A時，A使用格擋，攻擊判定失敗，不扣分。

當顯示器顯示到9，跑出藍色勝利 W。

當顯示器顯示到1，跑出紅色勝利 W。

程式模組說明:
output reg [7:0] R_color,//顯示紅色燈
output reg [7:0] G_color, //顯示綠色燈
output reg [7:0] B_color, //顯示藍色燈
output reg [3:0] column, //顯示燈亮的排
output reg a,b,c,d,e,f,g, //A玩家生命//B玩家生命
input a_up,a_down,a_left,a_right, //A玩家的移動(上下左右)
input b_up,b_down,b_left,b_right, //B玩家的移動(上下左右)
input MSB_in, CLK, Clear,//clear 初始值所有變數
input a_attack,a_defense, //A玩家的攻擊(a_attack)和防禦(a_defense)
input b_attack,b_defense//B玩家的攻擊(b_attack)和防禦(b_defense)

*測試影片https://drive.google.com/file/d/1d_-vRizJyCnW86-5cysBQkpCY3e9y5vr/view?usp=drivesdk
