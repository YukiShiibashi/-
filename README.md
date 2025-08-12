import excel using "C:\Users\yuki1\Downloads\卒業演習\計量経済学の第一歩\data\csv\2_income.xlsx", firstrow clear

/* 2A,2B 基礎統計表（分散を含む）を表にまとめる */
*　分散も計算したい場合は末尾に ",detail" をつける 

summarize income, detail
summarize yeduc, detail

/* 2C 共分散を求める */
correlate income yeduc, covariance

/* 2D 相関係数を求める　*/
correlate income yeduc



