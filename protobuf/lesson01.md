# 定义协议格式
示例：

    syntax = "proto2";
    package tutorial;
    option java_package = "com.example.tutorial";
    option java_outer_classname = "AddressBookProtos";

    message Person {
    required string name = 1;
    required int32 id = 2;
    optional string email = 3;

    enum PhoneType {
        MOBILE = 0;
        HOME = 1;
        WORK = 2;
    }

    message PhoneNumber {
        required string number = 1;
        optional PhoneType type = 2 [default = HOME];
    }

    repeated PhoneNumber phones = 4;
    }

    message AddressBook {
    repeated Person people = 1;
    }

## 数据类型
bool，int32，float，double，和string

## 修饰符
* required：必须提供该字段的值，否则该消息将被视为“未初始化”。尝试构建一个未初始化的消息将抛出一个RuntimeException。解析未初始化的消息将抛出一个IOException。除此之外，必填字段的行为与可选字段完全相同。
* optional：该字段可能已设置，也可能未设置。如果未设置可选字段值，则使用默认值。对于简单类型，您可以指定自己的默认值，就像我们type在示例中为电话号码所做的那样。否则，使用系统默认值：数字类型为0，字符串为空字符串，bools为false。对于嵌入式消息，默认值始终是消息的“默认实例”或“原型”，其中没有设置其字段。调用访问器以获取尚未显式设置的可选（或必需）字段的值始终返回该字段的默认值。
* repeated：该字段可以重复任意次数（包括零）。重复值的顺序将保留在协议缓冲区中。将重复字段视为动态大小的数组。

## 执行命令
    protoc -I=$SRC_DIR --java_out=$DST_DIR $SRC_DIR addressbook.proto