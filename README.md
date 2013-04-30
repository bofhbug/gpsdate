gpsdate
=======
/* The idea of this program is that you run it once at system boot time,
 * to set the local RTC to the time received by GPS.  Further synchronization
 * during system runtime is then handled by ntpd, interfacing with gpsd using
 * the ntp shared memory protocol.
 *
 * However, ntpd is unable to accept a GPS time that's off by more than four
 * hours from the system RTC, so initial synchronization has to be done
 * externally.  'ntpdate' is the usual option, but doesn't work if you're
 * offline.  Thus, this gpsdate utilith was created to fill the gap.
 */

clone from git://git.sysmocom.de/gpsdate.git
============================================================

/* gpsdate - small utility to set system RTC based on gpsd time 
 * (C) 2013 by sysmocom - s.f.m.c. GmbH, Author: Harald Welte
 * All Rights Reserved
 *
 * This program is free software; you can redistribute it and/or modify
 * it under the terms of the GNU General Public License as published by
 * the Free Software Foundation; either version 2 of the License, or
 * (at your option) any later version.
 *
 * This program is distributed in the hope that it will be useful,
 * but WITHOUT ANY WARRANTY; without even the implied warranty of
 * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 * GNU General Public License for more details.
 *
 * You should have received a copy of the GNU General Public License along
 * with this program; if not, write to the Free Software Foundation, Inc.,
 * 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 */

