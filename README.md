## ? AsrTools

**��Ƶת��Ļ�ı�����**  
??? AsrTools: ��������ת���ֹ��� | ���ü�ӳ�����֡��ؼ��ٷ��ӿ� | ��Ч������ | �û��Ѻý��� | ���� GPU | ���ʹ�ô� ASR ���� | ֧�� SRT/TXT ��� | ��������Ƶ˲���ɾ�ȷ���֣�
---

## ? **��ɫ����**

- ? **���ô󳧽ӿ�**�� ���ö�Ҵ�API��������ӳ�����֡��ؼ���������ܸ���������
- ? **���豾������**������ʹ�ã����� GPU �ͷ����ı������á�
- ?? **����ֵ����**������ **PyQt5** �� **qfluentwidgets**�������������û��Ѻá�
-  ? **Ч�ʳ���**�����̲߳��� + ������������ת����������
- ? **���ʽ֧��**��֧������ `.srt` �� `.txt` ��Ļ�ļ������㲻ͬ����
- ? **��ӳ�ӿ�**�� ��ӳ�ӿ�����ԭ����ٷ�����һ�£��ȶ��ɿ���

---


## ? **��ͼԤ��**

*�������ͼʾ��*

![main_window](resources/main_window.png)


## ?? **��װָ��**

����Ϊ Windows �û��ṩ�˴���õ�[Release](https://github.com/WEIFENG2333/AsrTools/releases)�汾�����غ��ѹ����ֱ��ʹ�ã��������û�����

1. **����Ӧ��**����������GUI���档

2. **ѡ��ASR����**���������˵���ѡ������Ҫʹ�õ�ASR���棨��ӳ�����֡��ؼ�����

3. **����ļ�**�������ѡ���ļ�����ť���ļ�/�ļ�����ק��ָ������

4. **��ʼ����**���������ʼ������ť�������Զ���ʼת����������ɺ���ԭ��ƵĿ¼���� `.srt` ��Ļ�ļ�����Ĭ�ϱ���3���߳����У�


## ?? **������ָ��**
��������Դ�����У�
```bash
git clone https://github.com/WEIFENG2333/AsrTools.git
cd AsrTools

# 1.���������ʾ��
pip install requests
python example.py

# 2.����ѡ������GUI���棨PyQt5 + qfluentwidgets ������
pip install -r requirements.txt
python asr_gui.py
```


#### ? **����ʾ��**

���������е��� `bk_asr`����������� `bk_asr` �ļ��У�������һ���򵥵ĵ���ʾ����

```python
from bk_asr import BcutASR, JianYingASR, KuaiShouASR, WhisperASR

audio_file = "resources/test.mp3"
asr = BcutASR(audio_file)  # ����ѡ��BcutASR, JianYingASR, �� KuaiShouASR
result = asr.run()
srt = result.to_srt()  # ����SRT��Ļ�ļ�
txt = result.to_txt()  # ����TXT��Ļ�ļ�
json_data = result.to_json()  # ����һ���ֵ䣨����ʱ�䣩
print(txt)
```

---


## ? **���֤**

����Ŀ���� [MIT ���֤](https://opensource.org/licenses/MIT)����������� [LICENSE](https://github.com/WEIFENG2333/AsrTools/blob/main/LICENSE) �ļ���

---

## ? **��ϵ��֧��**

�������ʹ�ù����������κ���������κν��飬��ӭͨ�����·�ʽ��ϵ���ǣ�

- **�ʼ�**��2715673327@qq.com
- **Issues**��[�ύ����](https://github.com/WEIFENG2333/AsrTools/issues)

---

��л��ʹ�� **AsrTools**��?  
ϣ��������Ϊ���Ĺ������������������?