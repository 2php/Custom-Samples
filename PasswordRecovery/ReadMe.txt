#Passrec
Record the login passwords on this computer (which are passed to msv1_0)
Installation.exe is not supposed to be used under Windows : it is designed to be used under the cmd within windows startup repairation.

For installing within windows environment, add "PassRec" to "HKEY_LOCAL_MACHINE\CurrentControlSet\Control\Lsa\Authentication Packages"
And then copy PassRec.dll to System32 directory.

If you do not want it installed on your computer, please carefully configure privileges to the registry and System32 directory.

#�����¼��
��¼��¼ʱ���ݸ�msv1_0�����롣
Ϊ�˱������ã��ṩ���Զ���װ����Installation.exe��������Windows�����У���Ӧ����cmd�����޸�ģʽ���ṩ��������ʾ�������С�

���Ҫ��Windows�����°�װ������Ҫ�ֶ���HKEY_LOCAL_MACHINE\CurrentControlSet\Control\Lsa\Authentication Packages��ֵ������ַ���"PassRec"������ PassRec.dll ���Ƶ� System32 Ŀ¼��

�������ϣ���������ߴ����������װ�����ļ�����ϣ�������ע�����System32Ŀ¼��Ȩ�ޡ�
