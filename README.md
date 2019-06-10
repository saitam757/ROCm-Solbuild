# ROCm-Solbuild
Trying to create packaging scripts for the [AMD Compute Stack](https://github.com/RadeonOpenCompute/ROCm) for Solus Linux eopkg,

Current Problem: Compiling HCC with error: Issue [here](https://github.com/RadeonOpenCompute/hcc/issues/1175)

Created packages and order of build:

1) Numactl: Status of building: Package created.

            "lseopkg numactl-2.0.12-1-1-x86_64.eopkg" yields:
                /usr/bin/memhog
                /usr/bin/migratepages
                /usr/bin/migspeed
                /usr/bin/numactl
                /usr/bin/numademo
                /usr/bin/numastat
                /usr/lib64/libnuma.so.1
                /usr/lib64/libnuma.so.1.0.0
                /usr/share/man/man2/move_pages.2
                /usr/share/man/man3/numa.3
                /usr/share/man/man8/migratepages.8
                /usr/share/man/man8/migspeed.8
                /usr/share/man/man8/numactl.8
                /usr/share/man/man8/numastat.8
                
            "lseopkg numactl-devel-2.0.12-1-1-x86_64.eopkg" yields: 
                /usr/include/numa.h
                /usr/include/numacompat1.h
                /usr/include/numaif.h
                /usr/lib64/libnuma.a
                /usr/lib64/libnuma.so
                /usr/lib64/pkgconfig/numa.pc
            
2) Roct:    ROCT-Thunk-Interface
            Status of building: Package created.
         
            "lseopkg ROCT-2.5.0-1-1-x86_64.eopkg" yields: 
                /usr/lib64/libhsakmt.so.1
                /usr/lib64/libhsakmt.so.1.0.6
                
            "lseopkg ROCT-devel-2.5.0-1-1-x86_64.eopkg" yields:
                /usr/include/hsakmt.h
                /usr/include/hsakmttypes.h
                /usr/include/linux/kfd_ioctl.h
                /usr/lib64/libhsakmt.so
                
3) Rocr:    ROCR-Runtime
            Status of building: Package created.
                
            "lseopkg ROCR-2.5.0-1-1-x86_64.eopkg" yields: 
                /usr/lib64/libhsa-runtime64.so.1
                /usr/lib64/libhsa-runtime64.so.1.1.9
                
            "lseopkg ROCR-devel-2.5.0-1-1-x86_64.eopkg" yields:
                /usr/include/hsa/Brig.h
                /usr/include/hsa/amd_hsa_common.h
                /usr/include/hsa/amd_hsa_elf.h
                /usr/include/hsa/amd_hsa_kernel_code.h
                /usr/include/hsa/amd_hsa_queue.h
                /usr/include/hsa/amd_hsa_signal.h
                /usr/include/hsa/hsa.h
                /usr/include/hsa/hsa_api_trace.h
                /usr/include/hsa/hsa_ext_amd.h
                /usr/include/hsa/hsa_ext_finalize.h
                /usr/include/hsa/hsa_ext_image.h
                /usr/include/hsa/hsa_ven_amd_aqlprofile.h
                /usr/include/hsa/hsa_ven_amd_loader.h
                /usr/lib64/libhsa-runtime64.so

4) Rocminfo:    ROCm Application for Reporting System Info 
                Status of building: Package created.
                
            "lseopkg rocminfo-1.0.0-1-1-x86_64.eopkg" yields: 
                /usr/bin/rocm_agent_enumerator
                /usr/bin/rocminfo
                
5) rocm_bandwidth_test: Bandwidth test for ROCm 
                        Status of building: Package created.
                        
            "lseopkg rocm_bandwidth_test-2.5.0-1-1-x86_64.eopkg" yields:
                 /usr/bin/rocm_bandwidth_test

         
         
         
