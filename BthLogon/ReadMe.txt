To install, Run the following commands with administrator privilege by order (under src directory).
��װ���Թ���Ա��Ȩ����ִ����������(��srcĿ¼��)��

nmake
nmake -install
install

Then, turn on bluetooth on both your computer and your phone, set your phone as discoverable, and start the configuration tool. Use the up/down arrows and Page up/down to select your phone, and press Enter to confirm. During configuration, you can press Esc to quit at and time, but you will need to finish the configuration later. If you can press F5 to re-discover the remote devices. 
Ȼ��򿪼������Զ���豸���������أ�������Զ���豸Ϊ�ɷ��֡�֮��������ù��ߡ������¼�/PageUp/PageDownѡ�������豸������Enter��ȷ�ϡ��ڹ����У������԰���ESC���˳�������֮���ٽ������á���������豸û�б����֣���Ҳ���԰���F5�����¼�����

Note that this project is just for fun and it provides no security. And, when bluetooth is turned off, the default action is to let any login attempts pass. Therefore, is you have any trouble logging in, you should switch your computer to flight mode, and then login.
ע�������߽������֡��������رյ�ǰ���£�һ�е�¼����Ĭ�Ϸ��С���������޷��������������ͨ����¼ҳ�����½ǵ��������ý����������������ģʽ���ٽ��е�¼��

To uninstall, run bin/uninstall.reg.
����ж�أ�������bin�ļ����е�uninstall.reg��

And you may need to manually remove SubAuth.dll under system32 directory.
���Ҫ����ɾ��������Ҫ��ж�غ�ɾ��system32Ŀ¼�µ�SubAuth.dll