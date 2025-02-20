[![spotify-github-profile](https://spotify-github-profile.kittinanx.com/api/view?uid=31sbmbau2z3vmv6j7ovwcrftbeze&cover_image=true&theme=natemoo-re&show_offline=false&background_color=000000&interchange=true&bar_color=53b14f&bar_color_cover=true)](https://spotify-github-profile.kittinanx.com/api/view?uid=31sbmbau2z3vmv6j7ovwcrftbeze&redirect=true)

```
#![no_std]
#![no_main]

use core::panic::PanicInfo;

#[no_mangle]
pub extern "C" fn _start() -> ! {
    let vga_buffer: *mut u8 = 0xb8000 as *mut u8;
    let hello: &[u8] = b"Hello!!";

    for (i, &byte) in hello.iter().enumerate() {
        unsafe {
            *vga_buffer.add(i * 2) = byte;
            *vga_buffer.add(i * 2 + 1) = 0x07;
        }
    }

    loop {}
}

#[panic_handler]
fn panic(_info: &PanicInfo) -> ! {
    loop {}
}
```

# Skills
![rust](https://img.shields.io/badge/Rust?style=for-the-badge&logo=rust&logoColor=white)
![python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![c](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white) 
![cpp](https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)

![arch](https://img.shields.io/badge/Arch_Linux-1793D1?style=for-the-badge&logo=arch-linux&logoColor=white) 
![zed](https://img.shields.io/badge/zedindustries-084CCF.svg?style=for-the-badge&logo=zedindustries&logoColor=white)
![git](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white) 
![pg](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white) 

# Baekjoon
[![solved.ac](http://mazassumnida.wtf/api/generate_badge?boj=enpotid)](https://solved.ac/profile/enpotid)
