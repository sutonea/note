# My Ruby note

## コーディングの方法

### 処理結果の返し方(案)

####ステータスコードと処理結果を構造体で返す

##### コード

    RET_CLASS = Struct.new(:status, :result)
    
    def my_proc_struct
      # 何らかの処理
      ret_obj =  RET_CLASS.new
      ret_obj.status = :succeed
      ret_obj.result = 'ステータスコード以外に返したい値'
      return ret_obj
    end

##### このように書いた理由

戻り値の取得時にタイプ数を減らしたかったから。

Structの場合 `ret_obj.status`

ハッシュの場合 `ret_obj[:status]`



##### 改善案

プロジェクト内で、戻り値の扱いを統一するのであれば、
すべての処理で共通のStruct(あるいはClass)を利用してもいいかもしれない。

- - -

####戻り値を配列で返す

##### コード

    def my_proc_array
      # 何らかの処理
      return [status, result]
    end
    
##### このように書いた理由

Structをわざわざ定義したくなかったから。
