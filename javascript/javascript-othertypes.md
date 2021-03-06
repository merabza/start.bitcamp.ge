# სხვა ტიპები

ჯავასკრიპტში არსებობს განსხვავება `null` \(non-value\) და `undefined` ტიპებს შორის, ეს უკანასკნელი აღნიშნავს - უმნიშვნელო ცვლადს. ანუ ცვლადი რომლისთვისაც მნიშვნელობა ჯერ არ მიგვინიჭებია. ცვლადებზე შემდგომში ვისაუბრებთ, მაგრმამ ჯავასკრიპტში შესაძლებელია ისეთი ცვლადების დეკლალირება, რომლებსაც მნიშვნელობა არ გააჩნიათ.

ჯავასკრიტპში ასევე შევხვდებით ბულეან \(boolean\) ტიპის ცვლადებსაც რომლებსაც მხოლოდ ორი `true` და `false` მნიშვნელობები გააჩნიათ და ამავადროულად ნებისმიერი მონაცემის გარდაქმნა შეიძლება ბულეანში:

```text
false, 0, ცარიელი სტრინგი(""), NaN, null და undefined, ყველა მიიღებს false მნიშვნელობას

ნებისმიერი სხვა მონაცემი კი გახდება true
```

ასეთი გარდაქმნის გაკეთება შეიძლება ```Boolean();`` ფუნქციით:

```text
Boolean(''); // false
Boolean(234); // true
```

მაგრამ, ასეთი ოპერაციის გაკეთება ძირითადად არ დაგჭირდებათ, როდესაც ბულეან მონაცემს ელოდებით, ჯავასკრიპტი მის კონვერსაციას ჩუმად მოახდენს. ამ მიზეზით, ხშირად მოისმენთ `true values, false values`, რაც ნიშნავს რომ მონაცემი ან `true` გახდება, ან `false` ბულეანში გარდაქმნის დროს.

ბულეანი ასევე მხარდაჭერას უწევს ლოგიკურ ოპერაციებსაც, მაგალითად: &&, \|\|, !, და ა.შ

