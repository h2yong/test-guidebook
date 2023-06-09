# 整型录入控件->允许Up-Down控件录入框
| 编号 | 输入/动作                                                    | 期望的输出/相应                                                                                                                            |
| :--- | :----------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------- |
| 1    | 录入数据的大小在【最小值，最大值】区间内，进行保存           | 保存成功                                                                                                                                   |
| 2    | 录入的数据等于【最小值】，进行保存                           | 保存成功                                                                                                                                   |
| 3    | 录入的数据等于【最大值】，进行保存                           | 保存成功                                                                                                                                   |
| 4    | 录入的数据等于【最小值】-1，进行保存                         | 1．保存不成功。弹出提示信息，并将焦点定位到当前录入框<br />或<br />2．当焦点移开当前录入框时，系统自动清空当前录入框的数据                 |
| 5    | 录入的数据等于【最大值】+1，进行保存                         | 1．保存不成功。弹出提示信息，并将焦点定位到当前录入框。<br />或<br />2．当焦点移开当前录入框时，系统自动清空当前录入框的数据。             |
| 6    | 录入的数据，带有小数位的数据                                 | 1．系统控制，不允许录入小数位。<br />或<br />2．录入小数位后，当焦点移开时，系统自动清空当前录入框数据。                                   |
| 7    | 录入空数据，进行保存                                         | 1．保存成功，保存后的值默认为0（允许为空）<br />2．保存不成功，弹出提示信息，确定后，将焦点定位到当前录入框（不允许保存空值）              |
| 8    | 在录入框录入字符内容，进行保存                               | 1．系统控制，不允许任何字符；<br />或<br />2．当焦点移开当前录入框时，系统自动清空当前录入框的字符内容。                                   |
| 9    | 录入正确数据后，显示结果                                     | 1．系统以带千分号格式显示数据。<br />2．数据全部居右显示。                                                                                 |
| 10   | 焦点跳转到当前录入框                                         | 数据被置为全选状态                                                                                                                         |
| 11   | 在录入框直接录入负数【前提：允许录入负数】                   | 录入中，在不需要任何键的辅助操作的情况下，就可以完成负数的录入                                                                             |
| 12   | 在整型录入框中，使用上箭头调整数据【基数=1】                 | 1．调整后的数据值 = 原值 + 基数的值                                                                                                        |
| 13   | 在整型录入框中，使用下箭头调整数据【基数=1】                 | 1．调整后的数据值 = 原值 - 基数的值                                                                                                        |
| 14   | 在整型录入框中，使用上箭头调整数据，使其调整到等于【最大值】 | 能正确操作                                                                                                                                 |
| 15   | 在整型录入框中，使用下箭头调整数据，使其调整到等于【最小值】 | 能正确操作                                                                                                                                 |
| 16   | 在整型录入框中，使用上箭头调整数据，使其调整到大于【最大值】 | 1．调整数据到最大值后，在使用上箭头调整时，系统不应该在做任何操作。<br />或<br />2．当焦点移开当前录入框时，系统自动清空当前录入框的数据。 |
| 17   | 在整型录入框中，使用下箭头调整数据，使其调整到小于【最小值】 | 1．调整数据到最小值后，在使用下箭头调整时，系统不应该在做任何操作。<br />或<br />2．当焦点移开当前录入框时，系统自动清空当前录入框的数据。 |