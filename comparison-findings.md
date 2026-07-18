Bu test synthetic və real istifadəçi davranışı arasında ciddi fərqləri göstərdi.

Synthetic test bəzi əsas problemləri düzgün tutdu. Xüsusilə dil baryeri, mikrofon istifadəsində tərəddüd və səhv etmək qorxusu həm AI, həm də real istifadəçidə müşahidə olundu. Bu, persona-da “beginner” səviyyə və “müəllimə” kimi detalların düzgün seçilməsinin nəticəsidir və AI-a doğru siqnal verdi. Həmçinin synthetic istifadəçi bəzi yerlərdə tərəddüd etsə də, ümumi flow-u davam etdirə bildi.

Lakin synthetic test bir çox kritik davranışı buraxdı. Real istifadəçi onboarding zamanı seçimləri tam başa düşmədiyi üçün təsadüfi qərar verdi və bir neçə dəfə kömək istədi. Seçimlərin mənasını anlamadığı üçün qərarı məntiqə yox, təsadüfə əsaslandı. Bundan əlavə, feedback hissəsində izahı oxumadan sadəcə “Continue” düyməsinə basdı və səhvin səbəbini anlamağa çalışmadı. Nəticə ekranında isə ümumiyyətlə dayanmadı və birbaşa çıxış etdi.

Synthetic istifadəçi isə bu mərhələlərdə daha səbirli və analitik davrandı, seçimləri oxuyaraq başa düşməyə çalışdı və feedback-i nəzərdən keçirməyə meyilli oldu. Bu fərq emosional və kontekstual faktorların synthetic testdə zəif əks olunması ilə bağlıdır.

Bəzi hallarda AI davranışı yanlış modelləşdirdi. Məsələn, istifadəçinin səhvdən öyrənəcəyini fərz etdi, lakin real istifadəçi öyrənmədən davam etdi. Bu, AI-nin istifadəçini olduğundan daha rasional və diqqətli təsəvvür etməsi ilə əlaqəlidir.

Hibrid nəticə göstərir ki, əsas problemlər dil baryeri, qeyri-aydın seçimlər, emosional narahatlıq, zəif feedback mexanizmi və istifadəçinin bəzi addımları ümumiyyətlə keçməsidir.

Bu təcrübə göstərir ki, synthetic testing ilkin analiz üçün faydalıdır, lakin real istifadəçi davranışını tam əks etdirmir. Xüsusilə beginner səviyyəsində olan istifadəçilər üçün real test mütləqdir.
