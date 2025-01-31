<p align='center'>
    <img src="https://capsule-render.vercel.app/api?type=waving&color=234567&height=300&section=header&text=Hello!&fontSize=90&animation=fadeIn&fontAlignY=38&descAlignY=51&descAlign=62"/>
</p>

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
![rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![c](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white) 
![cpp](https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)

![arch](https://img.shields.io/badge/Arch_Linux-1793D1?style=for-the-badge&logo=arch-linux&logoColor=white) 
![vim](https://img.shields.io/badge/VIM-%2311AB00.svg?&style=for-the-badge&logo=vim&logoColor=white) 
![git](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white) 
![pg](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white) 

