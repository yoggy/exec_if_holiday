# exec_if_holiday
## How to...
    $ crontab -l
    
    # 平日ダイヤ
    55 20 * * * ~/bin/exec_if_weekday say '次の鶴見線は21:08です'
    15 21 * * * ~/bin/exec_if_weekday say '次の鶴見線は21:28です'
    35 21 * * * ~/bin/exec_if_weekday say '次の鶴見線は21:48です'
    55 21 * * * ~/bin/exec_if_weekday say '次の鶴見線は22:08です'
    15 22 * * * ~/bin/exec_if_weekday say '次の鶴見線は22:28です'
    35 22 * * * ~/bin/exec_if_weekday say '次の鶴見線は22:48です'
    55 22 * * * ~/bin/exec_if_weekday say '次の鶴見線は23:08です。終電一本前です。'
    35 23 * * * ~/bin/exec_if_weekday say '次の鶴見線は23:48です。終電ですのでお乗り遅れにご注意ください'
    # 休日ダイヤ
    51 20 * * * ~/bin/exec_if_holiday say '次の鶴見線は21:03です。休日ダイヤですのでご注意ください。'
    23 21 * * * ~/bin/exec_if_holiday say '次の鶴見線は21:35です。休日ダイヤですのでご注意ください。'
    4  22 * * * ~/bin/exec_if_holiday say '次の鶴見線は22:16です。休日ダイヤですのでご注意ください。'
    46 22 * * * ~/bin/exec_if_holiday say '次の鶴見線は22:58です。終電一本前です。'
    35 23 * * * ~/bin/exec_if_holiday say '次の鶴見線は23:48です。終電ですのでお乗り遅れにご注意ください'

## Reference

  - [国民の祝日について - 内閣府](https://www8.cao.go.jp/chosei/shukujitsu/gaiyou.html)

## Copyright and license
Copyright (c) 2019 yoggy

Released under the [MIT license](LICENSE.txt)
