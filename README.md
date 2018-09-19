Gomoku

Ch??ng tr�nh game caro s? d?ng ?? h?a Turtle trong python v� engine AI d?a tr�n thu?t to�n minimax, c?t t?a alpha-beta ? hai c?p ?? s�u.

**Thu?t to�n**

1.Thu?t to�n Minimax

- Minimax l� m?t thu?t to�n ?? quy l?a ch?n b??c ?i k? ti?p trong m?t tr� ch?i 2 ng??i b?ng c�ch ??nh c�c gi� tr? cho c�c Node tr�n c�y tr� ch?i sau ?� t�m Node c� gi� tr? ph� h?p ?? ?i b??c ti?p theo.

- Hai ??i th? trong tr� ch?i ???c g?i l� MIN v� MAX lu�n phi�n thay th? nhau ?i. MAX ??i di?n cho ng??i quy?t d�nh th?ng l?i v� c? g?ng t?i ?a h�a ?u th? c?a m�nh, ng??c l?i ng??i ch?i ??i di?n cho MIN l?i c? g?ng gi?m ?i?m s? c?a MAX v� c? g?ng l�m cho ?i?m s? c?a m�nh c�ng �m c�ng t?t. Gi? thi?t ??a ra MIN v� MAX c� ki?n th?c nh? nhau v? kh�ng gian tr?ng th�i tr� ch?i v� c? hai ??i th? ??u c? g?ng nh? nhau.
M?i Node bi?u di?n cho m?t tr?ng th�i tr�n c�y tr� ch?i. Node l� l� Node ch?a tr?ng th�i k?t th�c c?a tr� ch?i.
Gi?i thu?t Minimax th? hi?n b?ng c�ch ??nh tr? c�c Node tr�n c�y tr� ch?i:
+ Node thu?c l?p MAX th� g�n cho n� gi� tr? l?n nh?t c?a con Node ?�.
   + Node thu?c l?p MIN th� g�n cho n� gi� tr? nh? nh?t c?a con Node ?�.
T? c�c gi� tr? n�y ng??i ch?i s? l?a ch?n cho m�nh n??c ?i h?p l� nh?t.
- N?u nh? ??t ??n gi?i h?n t�m ki?m (??n t?ng d??i c�ng c?a c�y t�m ki?m t?c l� tr?ng th�i k?t th�c c?a tr� ch?i).
- T�nh gi� tr? c?a th? c? hi?n t?i ?ng v?i ng??i ch?i ? ?�. Ghi nh? k?t qu?.
- N?u nh? m?c ?ang x�t l� c?a ng??i ch?i c?c ti?u (n�t MIN), �p d?ng th? t?c Minimax n�y cho c�c con c?a n�. Ghi nh? k?t qu? nh? nh?t.
- N?u nh? m?c ?ang x�t l� c?a ng??i ch?i c?c ??i (n�t MAX), �p d?ng th? t?c Minimax n�y cho c�c con c?a n�. Ghi nh? k?t qu? l?n nh?t.
2. Thu?t to�n c?t t?a alpha-beta.

- V� s? b�ng n? c�y tr� ch?i trong minimax n�n ta s? b? nh?ng n�t kh�ng t?i ?u b?ng c�ch c?t t?a alpha-beta.

- T? t??ng: + N?u m?t nh�nh t�m ki?m n�o ?� kh�ng th? c?i thi?n ??i v?i gi� tr? m� ch�ng ta ?� c�, th� kh�ng c?n x�t ??n h�m ?� n?a -> ti?t ki?m chi ph� th?i gian, b? nh? cho c�y t�m ki?m
		 + D�ng hai c?n Anpha v� Beta ?? so s�nh v� lo?i b? c�c tr??ng h?p s? kh�ng c?n x�t ??n trong thu?t to�n minimax.	

- M� t?: + Anpha l?u n??c ?i t?t nh?t c?a m�y, Beta l?u gi� tr? t?t nh?t c?a Ng??i ch?i
	   + N?u b?t c? khi n�o anpha >= beta, th� ng??i ch?i ch?c ch?n s? ch?n n??c ?i t?t nh?t cho h? v� c??ng b?c n??c ?i t?i h?n anpha cho m�y, v� v?y m� kh�ng c?n x�t th�m b??c n�o n?a

