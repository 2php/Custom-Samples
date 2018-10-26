For Installation:

1. Run nmake to build. Be sure to build with the suitable toolchain, for x86 dlls do not load under x64.
2.Copy the compiled dll "WelcomeMessager.dll" to System32 directory.
3.Import Register.reg
4.Customize the message with C:\Welcome.msg.
(Note:If you want to use a file with another path, please manually change the value HKEY_LOCAL_MACHINE\SOFTWARE\Welcome\Message)



About the format

C:\Welcome.msg is a file containing plain text.
Below are details about this file.
Each line should begin with a '@' and end with '##'
Next to the @, you are supposed to write a time filter. A time filter contains four parts separated by dots. 
And these parts are, from left to right, year, month, day of month, and day of week. You will be able to find more details if you go to see the MSDN document for SYSTEMTIME.
Each part is a single star '*', a number, or a (begin-end) segment.
And, after the time filter there comes a colon ':', and then the message.
And the program will search from the top of the file to the bottom.
For example, the following will be a legal file.
@*.10.(1-7).*:�������##
@*.12.7.*:�Լ�������������##
@*.*.*.*:Hello World!##



For Uninstallation:
1.Import uninstal.reg into the registry
2.Manually remove the WelcomeMessager.dll from system32 directory.
3.Manually remove the message configuration file C:\Welcome.msg.




��װ��

1.ִ��nmake����ע��ѡ����ϵͳλ��ƥ��Ĺ��߼���
2.��WelcomeMessager.dll������System32Ŀ¼��
3.����Register.reg��
4.��C:\Welcome.msg��������ʾ����Ϣ��
��ע�������׼���������ļ��������ã� ���޸� HKEY_LOCAL_MACHINE\SOFTWARE\Welcome\Message �е�·����



��Ϣ�����ļ���ʽ
C:\Welcome.msg ���ɴ��ı����ɵġ�������ʹ��notepad���κ��ı��༭�����б༭��
����Ϊ��ʽ����
ÿһ��Ӧ���� '@' ��ͷ���� '##' ��β��'��ʾ���ã�
�� @ ֮����Ӧ��ָ��һ��ʱ��ģʽ. ʱ��ģʽ�ɱ�.�ָ���Ĳ�����ɡ� �������α�ʾ���꣬�£��գ�������һ���еĵڼ��졣���ڼ�������㣬�����MSDN�Ϲ���SYSTEMTIME��������
ÿһ���ֿ�������������ģʽ֮һ��1)һ��*�ţ�2��һ������;3)һ����(���-�յ�)�������䡣
��ʱ��ģʽ֮��Ӧ����һ��:��֮����Ҫ��ʾ����Ϣ��
�����������½������䡣
�������µĳ���
@*.10.(1-7).*:�������##
@*.12.7.*:�Լ�������������##
@*.*.*.*:Hello World!##



ж�أ�
1.���� uninstal.reg
2.�ֶ���system32Ŀ¼�Ƴ� WelcomeMessager.dll
3.�ֶ�ɾ������������Ϣ�����ļ� C:\Welcome.msg.